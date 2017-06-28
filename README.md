# h5Lab

用于对h5相关项目学习研究

## 目录

- [每屏加载](https://github.com/since1984/h5Lab/tree/master/demo/demo01/demo01.md)

### 如何删除Git中的.DS_Store

> 删除项目中的所有.DS_Store。这会跳过不在项目中的 .DS_Store
> 1.`find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch`
> 将 .DS_Store 加入到 .gitignore
> 2.`echo .DS_Store >> ~/.gitignore`
> 更新项目
> 3.`git add --all`
> 4.`git commit -m '.DS_Store banished!'`

[原文链接]: (http://www.jianshu.com/p/fdaa8be7f6c3)

