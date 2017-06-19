# 创建一个github仓库
1. Repository name: 要创建git仓库的名子

1. Description: 这个仓库的简单描述, 让别人很快的了解这个库是做什么用的.

1. Public: 表示这个仓库是公开的, 任何人都可看到, 可以随意下载, 这就是传说中的开源.

1. Private: 私有库, 只能指定相关的人员才能看到并能下载. 这一般是公司或组织使用的私有项目, 这需要每个月向github交$7.

1. Initialze this Repository with a README: 初始生成README文件, .gitignore和license文件.
# 使用github仓库
## github仓库的使用
- 如果我们本地没有git仓库, 可以先在本地创建一个git仓库, 并做一个提交. 然后再互github远程仓库进行关联.
1. echo "# abc" >> README.md
2. git init
3. git add README.md
4. git commit -m "first commit"
5. git remote add origin https://github.com/wangleihd/freeBook-H5.git
6. git push -u origin master
- 我们本地已经有git仓库了, 那我们现在就直接与github仓库进行关联就可以了.
1. git remote add origin https://github.com/wangleihd/freeBook-H5.git
2. git push -u origin master
- 我们还可以用clone直接去下载这个项目, 这也是最常用下载或拉取github仓库的方法.
1. git clone https://github.com/wangleihd/freeBook-H5.git
# Markdown是一种轻量级标记语言
### 标题
- 使用#，可表示1-6级标题。
### 文字修饰符
- _你好_和*你好*   都是用来修饰字体不变
- **你好**和__你好__    用来修饰加粗
- ~~你好~~  表示这一行都删掉
### 列表
#### 无序列表
- 主要使用-和*来标记无序列表
#### 有序列表
- （1. 这里必须有一个空格）
### 段落
- 最末尾时空两个格表示换行
### 链接
- [github](http://github.com)
### 图片
- ![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png）
