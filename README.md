### Gitshell的简单使用

如果需要更多信息，[请移步](http://rogerdudler.github.io/git-guide/)

####clone
1.下载gitshell之后，在本地任意目录创建一个文件夹.我在d盘下新建了secbro文件夹

2.运行gitshell,利用如下命令切换到目标文件夹

<code>cd d:/secbro</code>

3. 运行命令，从Github下载项目到目标文件夹

  	<code>git clone /path/to/repository</code>
  	
  	<code>git clone https://github.com/secbro/gitshell-guide</code>
  	
运行结果：

![img](https://github.com/secbro/gitshell-guide/blob/master/images/cloneDone.jpg)

####remote

1) 运行 git remote

<code>git remote</code>

![img](https://github.com/secbro/gitshell-guide/blob/master/images/remote.jpg)

<code>git remote -v</code>

![img](https://github.com/secbro/gitshell-guide/blob/master/images/remotev.jpg)

2) 运行git remote add name [url],将你的仓库连接到某个远程服务器

<code>git remote add originSec https://github.com/secbro/gitshell-guide</code>

originSec可以换成任意你想要的名字，默认为origin

####add

**在使用add命令之前，你需要了解git工作流**

你的本地仓库由 git 维护的三棵“树”组成。第一个是你的 <code>工作目录</code>，它持有实际文件；第二个是 <code>暂存区（Index）</code>，它像个缓存区域，临时保存你的改动；最后是 <code>HEAD</code>，它指向你最后一次提交的结果。

[![img](https://github.com/secbro/gitshell-guide/blob/master/images/trees.png)](http://rogerdudler.github.io/git-guide/)

添加<code>工作目录</code>下的所有文件到<code>暂存区（Index）</code>

<code>git add .</code>

添加指定文件到<code>暂存区（Index）</code>

<code>git add git-shell-guide.html</code>

####commit

将修改后的文件提交，之后就可以使用push命令推送到远端仓库
<code>git commit -m "something"</code>

![img](https://github.com/secbro/gitshell-guide/blob/master/images/commit.jpg)

####push

<code>git push originSec</code>

输入账号和密码后，就可以提交项目到仓库啦!

![img](https://github.com/secbro/gitshell-guide/blob/master/images/lastStep.jpg)

命令行结果

![img](https://github.com/secbro/gitshell-guide/blob/master/images/theEnd.jpg)

网上仓库

![img](https://github.com/secbro/gitshell-guide/blob/master/images/repo.jpg)

####其他命令详解

**[LINKS](http://rogerdudler.github.io/git-guide/index.zh.html)**

