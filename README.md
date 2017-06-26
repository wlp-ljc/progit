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

* **git mv CONTRIBUTION.md mv.md** 实际上执行了三条指令
  * mv CONTRIBUTION.md mv.md
  * git rm CONTRIBUTION.md
  * git add mv.md



## 查看提交历史

* git log 查看所有提交历史

* git log -p 查看详细的更改信息

* git log -p -2 查看最近两次详细的更改信息

* git log —stat 查看最近的统计信息

* git log —pretty=online full fuller short 查看选项信息

  * git log —pretty=format 格式说明
  * %H 提交对象完整hash %h 提交对象简短hash
  * %T tree 完整哈希子串 %t tree 简短哈希子串
  * %P 父对象完整哈希子串 %p 父对象简短哈希子串
  * %an 作者            %ae 作者邮箱 %ad 作者修订日期 %ar 作者修改日期，按多久之前显示
  * %cn 提交者名字 %ce 提交者邮箱 %cd 提交提起 %cr 提交者 %s 提交说明

* git log 常用选项

  * -p 按格式显示每个更新的差异
  * — stat 显示每次更新的文件修改统计信息
  * —shortstat 只显示 最后的行数 添加移除统计
  * —name-only 仅在提交信息显示已修改的文件清单
  * —name-status 显示新增、修改、删除的文件清单
  * —abbrev-commit 仅显示hash1的前几个字符


## 撤销操作

* git commit —amend 保存上次未保存的信息



## 取消暂存的文件

* git reset HEAD mv.md 撤销暂存文件

  ​

## 取消对文件的修改

* git checkout — mv.md 取消对文件的修改

## 查看远程仓库

* git remote show origin




