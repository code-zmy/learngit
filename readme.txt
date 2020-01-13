Git is a version control system.
Git is free software.
git init 初始化一个Git仓库
git add filename 添加文件到Git库
git commit -m "提交信息" 提交完成

git status 查看当前仓库状态，哪些文件修改了没有提交
git diff filename 查看当前文件的修改内容

git log 显示从最近到最远的提交日志
git reflog 查看提交历史
git reset --hard commit_id 调到指定版本，HEAD为当前版本，HEAD^上个版本，HEAD~100上100个版本