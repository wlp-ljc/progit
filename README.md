git learn

## git 文件状态

* **untraccked file**
* **unmodified**
* **modified**
* **staged**



## 暂存已修改文件

* **git add**

* **git commit**

* **git status -s 短命令**


## git diff

* **git diff** 查看当前文件与暂存区域之间的差异
* **git diff —cached 或 git diff —staged** 查看暂存区与需要提交的内容之间的差异
* **git difftool —tool-help**  图形化插件

## 调过暂存区域

* **git commit -m** '提交更改'
* **git commit -a -m**  '调过暂存区域'

​    

## 移除文件

* **rm .md** 
* **git rm .md**
* **git rm -f** 强制删除，若已存在暂存区
* **git rm —cached .md** 工作文件保留  暂存区域删除



## 移动文件



