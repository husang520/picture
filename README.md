version https://git-lfs.github.com/spec/v1
oid sha256:7c09cf91d383edef851d955cc34a46f8b5ef64532f459bbfedb0377635e0555c
size 874

The following is the step of push large files by using git.

git init #创建本地仓库环境
git lfs install #安装大文件上传应用
git lfs track * #追踪要上传的大文件，*表示路径下的所有文件
git add .gitattributes #添加先上传的属性文件(要先上传属性文件，不然有可能失败)
git commit -m "first commit" #添加属性文件上传的说明
git remote add origin https://github.com/HITCSzwx/test.git  #建立本地和Github仓库的链接
git push origin master #上传属性文件
git add * #添加要上传的大文件，*表示路径下的所有文件
git commit -m "Git LFS commit" #添加大文件上传的说明
git push origin master #上传大文件

