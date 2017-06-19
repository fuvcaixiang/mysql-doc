# Vim的基本使用
- i：在当前字符的左边插入
- I：在当前行首插入
- a：在当前字符的右边插入
- A：在当前行尾插入
- o：在当前行下面插入一个新行
- O：在当前行上面插入一个新
- h: 向前移动一个字符
- j: 向下移动一行
- k: 向上移动一行
- l: 向后移动一个字符
- yy: 复制当前一行
- dd:剪切当前一行
- p: 粘贴内容到游标之后（粘贴10次10p）
- P: 粘贴内容到游标之前
# 基本的文件操作
- 文件的创建、删除、复制、重命名、移动
- 列出文件列表
- 查看文件内容
1. touch  file(创建文件)
2. cp file file1（复制文件）
3. cp file  /home/linux/file1
4. mv file   file2（移动文件）
5. mv file  /home/linux/
6. ls -al  .（列出文件名）
7. cat  file（查看文件内容）
# 基本的目录操作
- 目录的创建、删除、复制、重命名、移动
- 列出目录列表
- 目录中查找文件
1. mkdir dir
2. cp dir   dir1  -a
3. cp dir   /home/linux/dir2  -a
4. mv dir  dir2
5. mv dir  /home/linux/
6. rm  dir  -rf
7. ls -d  dir
8. find  ./dir  -name  "filename"
# 文件的归档和压缩
- 使用gzip和gunzip对文件进行压缩和解压缩
- 使用bzip2和bunzip2对文件进行压缩和解压缩
- 使用tar对文件和目录进行压缩和解压缩
1. gzip  filename
2. bzip2  filename
3. gunzip filename
4. bunzip2  filename
5. tar czvf  file.tar.gz dir
6. tar cjvf  file.tar.bz2 dir
7. tar cJvf  file.tar.xz  dir
8. tar xvf  file.tar.gz
9. tar xvf  file.tar.xz
