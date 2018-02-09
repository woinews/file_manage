# read_csvfile
用pandas读取CSV文件有时会报错，这里把经常出错的点整理了下：
1、读取CSV指定路径不能包含中文，有可能导致初始化失败；
2、如果是用斜杠表示路径时，遇到U开头或数字的文件夹要多加一斜杠（\\user、\\001.csv）
3、编码报错问题，要指定编码，常用的编码有ansi、utf8、gbk等
pd.read_csv(filepath,encoding = 'ansi')
4、以字符串形式读入时，要指定dtype参数为str
pd.read_csv(filepath,encoding = 'ansi',dtype = str)
