# Gut_args
比如0.1 prevalence  过滤在所有样本中低于10%的菌群。  

## prevalence：  
### 16S：  
   人prevalence：0.1  
   小鼠prevalence：0.2  
### 宏数据：
   人prevalence：0.1  
   小鼠prevalence：0.3  

## TSS
### 如果TSS数据：  
 core(pseq.sub, detection = 0.01, prevalence = .1)  
 我对detection理解是，tax表中的每个数值都必须大于0.01才会保留  

### 如果是rawconut数据：  
 core(pseq.sub, detection = 1, prevalence = .1)  
 我对detection理解是，tax表中的每个数值都必须大于1才会保留  

### kraken2输出
kraken2输出是TSS的结果  
1 deseq得方法不适合  
2 lefse选择CPM也可以分析，意思是Kraken2输出一个数值为0.01，其实在计算中选用CPM就是进行了转化成10000  
3 linda就是个线性回归，counts,他就用negative binomial regression；percent, 他就直接用gaussian regression,也就是我们通常做的那样。  
4 非参数可以直接做  


# ncbi_vs_gtdb_r214  菌种分类对应关系
https://data.gtdb.ecogenomic.org/releases/release214/214.1/auxillary_files/ncbi_vs_gtdb_r214_bacteria.xlsx

# 酶对应菌的关系
http://eggnog5.embl.de/#/app/home  
Metacyc


# metaphlan to GTDB
http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases/mpa_vOct22_CHOCOPhlAnSGB_202212_species.txt.bz2  
https://github.com/biobakery/MetaPhlAn/blob/master/metaphlan/utils/mpa_vOct22_CHOCOPhlAnSGB_202212_SGB2GTDB.tsv  


# 多样性
Shannon指数更加敏感于物种的均匀度，即各物种在群落中的相对比例。  
Simpson指数更加关注物种的丰富度和优势物种的存在，它给予丰度较高的物种更大的权重。  
Chao1指数是一种估计群落中未被观察到的物种总数的方法，主要用于评估物种的丰富度。  

