### ps命令的使用

ps 显示瞬间进程信息，如过想对进程进行==实时监控==，应该使用==top==命令

常用参数组合

1. `ps -aux`

- -a : 所有进程都显示 
- -u : 以用户为主的进程状态
- -x : 列出比较完整信息，通常与-a配合

2. `ps -ef `
- -e : 与-a具有同样效果
- -f : 更完整的输出，与-x类似


**常与grep配合使用**
grep 与 egrep 的区别

grep: 基本正则表达式
egrep: 拓展正则表达式

grep -E 等同于 egrep ，参数为正则表达式

```
cat kuaishou01.log | grep -E 'piece [0-9]* size [0-9]* send'
cat kuaishou01.log | egrep 'piece [0-9]* size [0-9]* send'
```








