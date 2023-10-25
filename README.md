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

# ncbi_vs_gtdb_r214  菌种分类对应关系
https://data.gtdb.ecogenomic.org/releases/release214/214.1/auxillary_files/ncbi_vs_gtdb_r214_bacteria.xlsx

# 酶对应菌的关系
http://eggnog5.embl.de/#/app/home  
Metacyc
