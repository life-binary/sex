## wget 基本使用

wget就是一个下载器，可以下载参数对应的地址的文件

1. 下载文件
`wget https://wordpress.org/latest.zip`

----

2. 下载后保存到指定目录 ==-P==
`wget -P /opt/wordpress https://wordpress.org/latest.zip`

----

3. *断点续传*  ==-c==
`wget -c https://wordpress.org/latest.zip`  
有时候下载某文件，网络中断后，可以用“-c”来继续之前的下载，如果不使用“-c“则表示重新开始整个下载，且在下载的文件后面加".1"，因为之前没有下载完的文件还存在。  
----

4. *对于大文件* ==-b==
`wget -b http://example.com/big-file.zip`
可以用“-b”参数在后台下载，输出信息会保存在同目录的“wget-log”中，你可以用`tail -f wget-log`来查看。

