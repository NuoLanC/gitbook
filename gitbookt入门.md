```shell
## 进入需要放的目录，下载刚刚初始化好的github项目
MacBook:testgit xhchen$ git clone https://github.com/NuoLanC/gitbook.git
Cloning into 'gitbook'...
warning: You appear to have cloned an empty repository.
## 查看已安装的gitbook 版本
MacBook:gitbook xhchen$ gitbook -V
CLI version: 2.3.2
GitBook version: 3.2.3
## 初始化gitbook 版本
MacBook:gitbook xhchen$ gitbook init
[0;36minfo:[0m create SUMMARY.md 
[0;36minfo:[0m initialization is finished 
MacBook:gitbook xhchen$ ll
total 16
drwxr-xr-x   5 xhchen  staff  160  8  1 20:28 ./
drwxr-xr-x   5 xhchen  staff  160  8  1 20:27 ../
drwxr-xr-x  10 xhchen  staff  320  8  1 20:27 .git/
-rw-r--r--   1 xhchen  staff   16  8  1 20:28 README.md
-rw-r--r--   1 xhchen  staff   40  8  1 20:32 SUMMARY.md
## 启动gitbook 服务 并在浏览器中打开 http://localhost:4000 可看到示例
MacBook:gitbook xhchen$ gitbook serve
Live reload server started on port: 35729
Press CTRL+C to quit ...

[0;36minfo:[0m 7 plugins are installed 
[0;36minfo:[0m loading plugin "livereload"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "highlight"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "search"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "lunr"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "sharing"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "fontsettings"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "theme-default"... [0;32mOK[0m 
[0;36minfo:[0m found 1 pages 
[0;36minfo:[0m found 0 asset files 
[0;36minfo:[0m [0;32m>> [0mgeneration finished with success in 0.4s ! 

Starting server ...
Serving book on http://localhost:4000
## 编译到指定的目录
MacBook:gitbook xhchen$ gitbook build . docs
[0;36minfo:[0m 7 plugins are installed 
[0;36minfo:[0m 6 explicitly listed 
[0;36minfo:[0m loading plugin "highlight"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "search"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "lunr"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "sharing"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "fontsettings"... [0;32mOK[0m 
[0;36minfo:[0m loading plugin "theme-default"... [0;32mOK[0m 
[0;36minfo:[0m found 1 pages 
[0;36minfo:[0m found 0 asset files 
[0;36minfo:[0m [0;32m>> [0mgeneration finished with success in 0.4s ! 
## git 添加所有
MacBook:gitbook xhchen$ git add *
## git 注释
MacBook:gitbook xhchen$ git commit -m"优化"
[master (root-commit) 20f0a57] Inital commit
## 提交到github上
MacBook:gitbook xhchen$ git push -u origin master
## 然后输入github 账号
Username for 'https://github.com': 366690712@qq.com
## 输入账号对应的密码
Password for 'https://366690712@qq.com@github.com':

To https://github.com/NuoLanC/gitbook.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
##
```
