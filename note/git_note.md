### 配置Git
```bash
git config --global user.name = "hbzgfcq"
git config --global user.email = "hbzgfcq@163.com"
```
### 创建版本库
```bash
mkdir learngit
cd learngit
git init
```
### 向版本库中添加文件
```bash
vi readme.txt
git add readme.txt
git commit -m "wrote a readme file"
```
### 查看版本库的状态
```bash
git status
```
### 检查文件的变化
```bash
git diff readme.txt
```
### 查看Git日志
```bash
git log
```
### 查看Git的命令日志
```bash
git reflog
```
### 后退到上一个版本
```bash
git reset --hard HEAD^
```
### 后退到上上个版本
```bash
git reset --hard HEAD^^
```
### 后退到上100个版本
```bash
git reset --hard HEAD~100
```
### 后退到某个版本
```bash
git reset --hard versionNumber
```
### 撤销对工作区中的文件的修改
```bash
git checkout -- readme.txt
```
### 删除工作区中的一个文件
```bash
rm test.txt
```
### 从版本库中删除它
```bash
git rm test.txt-u
git commit -m "remove test"
```
### 撤销在工作区中删除文件的操作
```bash
git checkout -- test.txt
```


### 生成密钥对
```bash
ssh-keygen -t rsa -C "hbzgfcq@163.com"
```
### 为你的GitHub账号添加公钥
### 查看远端仓库
```bash
git remote -v
```
### 将本地版本库和GitHub上的一个远程库关联
```bash
git remote add origin git@github.com:hbzgfcq/learngit.git
```
### 从远程版本库中拉取代码到本地库
```bash
git pull origin master
```
### 将本地库中的所有内容推送到远程库上
```bash
git push -u origin master
```
### 将远程库克隆到本地
```bash
git clone git@github.com:hbzgfcq/learngit.git
```
### 克隆时报错：文件名太长，解决方法如下
```bash
git config --system core.longpaths true
```
