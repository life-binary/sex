#### netstat 命令的使用

netstat -natp 显示tcp、udp的==端口==和==进程==等相关情况

recv | send | local address | foreign address | stata
接受/发送 字节数  本地地址 ip+port  远端地址    状态

- -t (tcp) 仅显示tcp相关选项
- -u (udp)仅显示udp相关选项
- -n 拒绝显示别名，能显示数字的全部转化为数字
- -l 仅列出在Listen(监听)的服务状态
- -p 显示建立相关链接的程序名


1. 列出所有连接
`netstat -a`
2. 列出所有tcp连接
`netstat -at`
3. 只列出监听中的队列
`netstat -atl`

mac下：-p 参数需要指定协议
`netstat -natp tcp`

==但是Mac下还是不能直接显示程序名program==
- 解决方法：配合lsof 查看端口号，可以看到进程名


