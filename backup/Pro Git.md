Git使用指南，免费开源书籍。[https://git-scm.com/book/zh/v2](https://git-scm.com/book/zh/v2)
## 关于Git的一些笔记
别人总结的好笔记：
https://www.cnblogs.com/mq0036/p/17082938.html
### Git重要概念和名称
![image](https://github.com/user-attachments/assets/3e82fadb-cca4-47b5-9095-e25197324246)
![image](https://github.com/user-attachments/assets/6818868b-d274-424a-ad53-147f04726520)
### Git基本流程
0、准备仓库：创建或从服务端克隆一个仓库。
1、搬砖：在工作目录中添加、修改代码。
2、暂存（git add）：将需要进行版本管理的文件放入暂存区域。
3、提交（git commit）：将暂存区域的文件提交到Git仓库。
4、推送（git push）：将本地仓库推送到远程仓库，同步版本库。
5、获取更新（fetch/pull）：从服务端更新到本地，获取他人推送的更新，与他人协作、共享。
git commit -a指令省略了add到暂存区的步骤，直接提交工作区的修改内容到版本库，不包括新增的文件。
git fetch、git pull 都是从远程服务端获取最新记录，区别是git pull多了一个步骤，就是自动合并更新工作区。
git checkout .、git checkout [file] 会清除工作区中未添加到暂存区的修改，用暂存区内容替换工作区。
git checkout HEAD .、git checkout HEAD [file] 会清除工作区、暂存区的修改，用HEAD指向的当前分支最新版本替换暂存区、工作区。
git diff 用来对比不同部分之间的区别，如暂存区、工作区，最新版本与未提交内容，不同版本之间等。
git reset是专门用来撤销修改、回退版本的指令，替代上面checkout的撤销功能。


