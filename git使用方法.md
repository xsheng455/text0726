 ##  git init 初始化文件夹，默认被隐藏
1. git add 文件名
2. git commit -m "注释"
3. git commit  错误退出 -- Esc+:q(!)
4. git status 查看文件是否改变,保存到版本库
5. git add ./  将当前文件夹下所有修改过的文件全部提交
6. git commit --all -m "注释"  把所有修改过的文件放到版本库
7. git .gitignore 这个文件可以设置要被忽略的文件
在.gitignore中可以写被忽略的文件的路径，以/开头一行写一个路径
建立方法  .gitignore.
8. git log  查看提交记录
9. git log --oneline  查看显示一行
10. git reset --hard Head~0 最后面的数字表示回退的次数，0表示最近的一次
11. git reset --hard 版本号   指向要回退的版本
12. git reflog 显示版本切换的记录
13. git branch 分支名 创建分支（默认主分支 master）
14. git checkout 分支名  切换主分支
15. git merge 分支名  合并到主分支
16. git branch 可以查看当前有多少分支











