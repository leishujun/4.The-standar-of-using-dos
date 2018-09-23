# The-standar-of-using-dos
# __命令的正确使用方式__  

command  选项  参数  

比如：   

date  -d  “-1 day”  

date就是命令  
-d就是选项  
“-1 day”就是参数  


想要执行多个命令又不想分开执行  （就是用分号放在两个命令之间）
ls；date；cat /etc/sysyconfig/network-scripts/ifcfg-ens33  

想要执行多个命令又不想分开执行，且知道命令执行是否成功可以这么操作  （就是在命令之间放上两个&&）

ls&&date&&nl /etc/sysyconfig/network-scripts/ifcfg-ens33  

想优雅的装逼还可以这么操作 （就是用反斜杠把命令分开成绩部分） 

ho\\

st\\

name

显示出来的是你的主机名字

# __终端__  

涉及命令ssh（有双向、许多电脑相互之间免密登陆）,chvt（切换终端）,tty,w,who,whoami,who am i，screen等等  

一般tty的都是本地用户登陆  ，pts的都是远程计算机登陆

# __bash shell__  

显示当前的使用的shell语言echo ${SHELL}  

查看系统支持的shell语言cat /etc/shells  

直接输入/bin/sh就可以切换为sh语言，其他的系统语言类似

# __修改命令提示符__  

PS1="\[\e[1;5;41;33m\][\u@\h \W]\\$\[\e[0m\]"  

如何使用详情请查看

man bash

然后搜索

/PS1
