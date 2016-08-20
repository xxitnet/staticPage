# 如何发布静态页面到github上

1. 创建一个新创库   cretae new Reponsitory

 勾选Initialize this repository with a README的区别

 勾选：会在master分支上创建创库

 不勾选：到时候会在gh—pages分支上

2. 创建github页面并发布

    settings->Automatic page generator   此时会在gh-pages分支上出现了我们创建的静态页面项目

3.  创建本地创库并初始化
```
mkdir demo && cd demo
git init
```

4. 关联远程仓库
```
git remote add origin   ghihub仓库地址
```

5. 把远程创库gh-pages分支拉取下来
```
git pull origin gh-pages
```

6. 删除拉取下来不需要的文件，把我们自己的文件到这个目录

7. 本地创建分支gh-pages 并提交
```
git branch gh-pages
git checkout gh-pages
git add -A
git commit -m"commit“
```

8. 推送本地仓库到远程gh-pages下
```
git push -u origin gh-pages
```
