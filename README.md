# file_manage
## 1、join_csv.py
  用pandas读取CSV文件有时会报错，这里把经常出错的点整理了下：   
  1、读取CSV指定路径不能包含中文，有可能导致初始化失败  
  2、如果是用斜杠表示路径时，遇到U开头或数字的文件夹要多加一斜杠（\\\user、\\\001.csv）   
  3、编码报错问题，要指定编码，常用的编码有ansi、utf8、gbk等   
  pd.read_csv(filepath,encoding = 'ansi')   
  4、以字符串形式读入时，要指定dtype参数为str   
  pd.read_csv(filepath,encoding = 'ansi',dtype = str)   

## 2、join_xls.py
  用pandas合并excel文件  
  
## 3、connector_mysql.py
  使用mysql-connector库连接本地mysql数据库进行数据处理  
  
## 4、connect_mongodb.py
  使用远程连接，将json数据上传至mongodb中





