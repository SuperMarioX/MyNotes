## 常用的cmd命令
### 1. git删除提交的文件
```
git rm -f files
git commit -m "remove added files"
git push
```

### 2. 将一个文件夹下的所有文件名添加到某文件
```
find /home/user -type f > out.txt
```