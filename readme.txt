Git is a version control system.
Git is free software.
git init 初始化一个Git仓库
git add filename 添加文件到Git库
git commit -m "提交信息" 提交完成

git status 查看当前仓库状态，哪些文件修改了没有提交
git diff filename 查看当前文件的修改内容

git log 显示从最近到最远的提交日志 --pretty=oneline
git reflog 查看提交历史
git reset --hard commit_id 调到指定版本，HEAD为当前版本，HEAD^上个版本，HEAD~100上100个版本

场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- filename
场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD filename，就回到了场景1，第二步按场景1操作。
场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。