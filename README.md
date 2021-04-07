# git-github-
git / github基础知识和命令

知识点引用： https://blog.csdn.net/hanhailong726188/article/details/46738929
第一步：建立git仓库
cd到你的本地项目根目录下，执行git命令

git init

第二步：将项目的所有文件添加到仓库中

git add .

如果想添加某个特定的文件，只需把.换成特定的文件名即可

第三步：将add的文件commit到仓库

git commit -m "注释语句"
第四步：去github上创建自己的Repository，创建页面如下图所示：

第五步：重点来了，将本地的仓库关联到github上

git remote add origin https://github.com/hanhailong/CustomRatingBar
后面的https链接地址换成你自己的仓库url地址，也就是上面红框中标出来的地址

第六步：上传github之前，要先pull一下，执行如下命令：

git pull origin master
敲回车后，会执行输出类似如下
第七步，也就是最后一步，上传代码到github远程仓库

git push -u origin master
执行完后，如果没有异常，等待执行完就上传成功了，中间可能会让你输入Username和Password，你只要输入github的账号和密码就行了


…or create a new repository on the command line
echo "# test-demo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/herry-deng/test-demo.git
git push -u origin master


…or push an existing repository from the command line
git remote add origin https://github.com/herry-deng/test-demo.git
git branch -M master
git push -u origin master
