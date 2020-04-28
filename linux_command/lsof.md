### lsof 命令的使用

lsof (list open files) 列出当前系统打开的文件信息，可以查看端口占用情况

==lsof -i 需要root权限==
1. 查看8000端口是否被占用
`lsof -i:8000`
2. 显示进程现在打开的文件
`lsof -c nginx`
`lsof -p 18616` 根据pid




