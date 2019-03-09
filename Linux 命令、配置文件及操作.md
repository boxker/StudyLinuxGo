## Linux 命令、配置文件及操作

## 命令

命令|参数|说明
-|-|-
**A**||
alias、unalias||命令别名
**B**||
**C**||
cat||查看文件内容
cd||切换目录
chown||修改拥有着
chgrp||修改所属组
chmod||修改模式权限
clear||清屏
cp|-a 等价 -dpR<br>-d 保留文件链接<br>-p 属性不变<br>-r/R 递归|复制
**D**||
dd|if 输入文件<br>of 输出文件<br>count 块数量<br>bs 块大小（字节）|拷贝[详情](https://www.cnblogs.com/jikexianfeng/p/6103500.html)
date|+%m/%d/%y 按月日年<br>+%y-%m-%d:%k:%M:%S格式为 年月日时分秒<br>无参数显示时间|
df|-m 以MB为单位（默认为KB）|查看文件系统
du||查看目录大小
**E**||
echo||显示信息
env||环境变量
export||输出变量
exit||退出shell会话
**F**||
fdisk|-l 显示信息<br>交互模式<br>d 删除一个分区<br>n 新增一个分区<br>p 显示分区表<br>q 退出<br>t 改变分区号码<br>w 保存|分区工具
fuser|-k 终止访问的进程|查看那些进程在访问该文件系统
fsck|-y 自动修复任何错误|修复文件系统
**G**||
grep||过滤信息
groupadd||添加组
groupmod|-G 编辑组成员|修改组信息
groupdel||删除组
groups||显示组信息
gpasswd||修改组密码
**H**||
halt||停止
history||历史
hostname|新名称（重启无效）<br>无参数显示主机名|
**I**||
id||查看当前用户信息
**J**||
**K**||
**L**||
logout||退出登录
ls|-a 所有，包括隐藏<br>-l 列表（简写ll）<br>-R 递归列出所有子文件目录<br>-t 时间排序|
ln|-s 符号链接<br>无参硬连接|链接
logname||登录名称
lsof||查看那些进程在访问该文件系统
**M**||
man|man name|查看帮助
mesg||
mv|-f 强行覆盖|移动、改名
man||帮助
mount||挂载
more||分页显示
mkdir||创建文件夹
mkfs||创建文件系统
**N**||
newgrp||切换组
**O**||
**P**||
passwd|-d 删除密码<br>-l 锁定<br>-u 解锁|更改密码
parted||分区工具
pwd||当前目录
ps|-ef 简要<br>-aux 详细|
pwck||检查密码文件格式
**Q**||
**R**||
rm|-r 递归<br>-f 强制|删除文件
rpm|-ivh 安装<br>-Uvh 升级<br>-e 卸载<br>-aq 查看所有已安装<br>-iq 查询<br>-f 查看属于那个文件|包管理工具
**S**||
shutdown||关机
su||切换用户
startx||启动X桌面
**T**||
tail|-f 显示末尾|实时查看文件内容
touch||创建文件
tar|-cvf 打包<br>-xvf 解压<br>-z 使用gzip<br>-v 显示信息<br>-f 指定名称
**U**||
uname||
useradd|-D 修改配置文件|添加用户
usermod||修改用户信息
userdel|-r 同时删除目录|删除用户
umount||取消挂载
unzip|-l 查看文件清单<br>-v 查看执行信息|
**V**||
**W**||
who||查看当已前登录用户
whoami||查看当前会话用户
write||发送信息
wc|-l只显示行数<br>行数 单词数 字节数 文件名|统计
**X**||
**Y**||
**Z**||
zip|-m 安装后删除源文件<br>-r 目录下所有一同处理<br>-S 半酣系统文件及隐藏文件<br>-l 查看报包含内容<br>-v 哈坎执行信息|



## 配置文件

文件|用途|备注
-|-|-
/etc/lilo||
/etc/rc.d/rc.local|启动脚本|
/etc/shadow|用户信息（密码md5）|
/etc/passwd|用户信息|
/etc/default/useradd|用户配置文件|
/etc/fatsb|自动挂载文件|

## 操作

### 1.安装系统
操作|说明
-|-
alt + F1|安装程序主窗口
alt + F2|shell环境
alt + F3|调试信息
alt + F4|OS核心信息
alt + F5|mke2s的输出信息

### 2.shell环境

变量|用途
HOME|
LOGNAME|
MAIL|
MAILCHECK|
PATH|
PS1|
PS2|
LANG|

### 3.默认umask

类型|umask
-|-
目录|777
文件|666

### 4.源码编译安装

```
1 ./configure
2 make
3 make install
```


[有道云笔记链接](http://note.youdao.com/noteshare?id=db7838e27993434d54e9c94aae3e4abb)

[博客园](https://www.cnblogs.com/cjb100/p/10502703.html)

[GITHUB](https://github.com/boxker/StudyLinuxGo)
