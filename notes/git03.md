## 创建本地git版本库

####Git初始化设置
```
#git config --global user.name 'zaifeng'
#git config --global user.email 'zhaozaifeng@360.cn'
#git config --global color.ui true
```

####创建一个本地版本库
```
#git init [repository]
```

####添加文件本地版本库
```
#git add file1

#git add file1 file2 ... fileN

#git add .

```

####提交文件到本地版本库
```
#git commit --message "code commit"  

#git commit -m "code comments"
```

什么？懒？两步提交太麻烦

```
#git commit -a -m "code comment"
```

有什么问题？