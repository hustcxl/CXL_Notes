# git&github Notes :see_no_evil:
## git 常用命令速查
* git 将远程仓库同步到本地
```bash
# git fetch origin master
# git merge origin/master
 
```
## 一些参考教程

* [史上最简单的 GitHub 教程](https://blog.csdn.net/qq_35246620/article/details/66973794) 感谢@维C果糖 附[github地址](https://github.com/guobinhit)
* [git 提交到github不显示贡献值的问题解决](https://my.oschina.net/zlhblogs/blog/3003282)  
  * 关键步骤1，查看本地git用户名和邮箱
  ```
  $ git config --global user.name
  $ git config --global user.email
  ```
  * 关键步骤2，配置git用户名和密码，使其与远程GitHub一致
  ``` 
  $ git config --global user.name “github’s Name”
  $ git config --global user.email "github@xx.com"
  ```
* [git 入门教程](http://rogerdudler.github.io/git-guide/index.zh.html)

* [GitHub 项目徽章的添加和设置](https://lpd-ios.github.io/2017/05/03/GitHub-Badge-Introduction/)   
* [GitHub与Jupyter Notebook、GitHub page、CSDN博客大联动](https://www.jianshu.com/p/c4dd47a33daa)

[<<返回主目录](../README.md)
