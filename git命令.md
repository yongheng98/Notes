# Git命令

`git init` 创建一个本地仓库。成功时，会在目录下新增一个 **隐藏格式的** `.git`的文件

[本地连接GitHub教程](https://www.cnblogs.com/zeo-to-one/p/8367801.html)



`git config --global user.name "yongheng98"` 全局配置用户名

`git config --global user.email "1017029364qq.com"` 全局配置邮箱

` ssh-keygen -t rsa -C "1017029364@qq.com"` 生成邮箱配对的SSH

![image-20211102211327680](https://i.loli.net/2021/11/02/YlVJgeaE6LurkIp.png)

遇到冒号就按空格，共按三次。

找到生成的`id_rsa.pub`文件，复制下来。

粘贴到`GitHub`网页版的setting->SSH and GPG->new SSH key,粘贴进去



`ssh -T git@github.com` 测试是否连接成功github，成功会有提示。

`ssh -T git@gitee.com` 测试是否连接成功码云，成功会有提示。

![image-20211102211933816](https://i.loli.net/2021/11/02/k2GwT4SYULJezZi.png)



```git
git status   // 查看工作目录的状态
git add <file> // 将文件添加到暂存区
git commit -m "zhushi" // 提交更改，添加备注信息（此时将提交信息提交给本地仓库）
git push origin master // 将本地仓库的文件push到远程仓库（若push不成功，可以加-f 进行强推操作）
```

以后，只需要`git push`

