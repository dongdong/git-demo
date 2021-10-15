### Git cmd demo


##### basic cmds
    * information:
        - git status
        - git config --list
        - git config -e
        - git log
        - git reflog
    * basic operation:   
        - git init
        - git add [file1] [file2] ...
        - git add .
        - git rm [file1] [file2] ...
        - git rm --cached [file]
        - git mv [file-original] [file-renamed]
        - git commit -m [message]
        - git commit --amend -m [message]
        - git reset --hard [commit]


##### branch cmds
    * branch cmds:
        - git branch
        - git branch [branch-name]
        - git checkout [branch-name]
        - git checkout -b [branch-name]
        - git branch [branch-name] [commit]
        - git checkout -
        - git branch -d [branch-name]
    * remote branch
        - git branch -r
        - git branch --track [branch] [remote-branch]
        - git branch --set-upstream [branch] [remote-branch]
        - git branch -dr [remote-branch]
    * branch merge
        - git merge [branch]
        - git merge --no-ff [branch]
        - git cherry-pick [commit]


##### tag cmds
    * tag cmds
        - git tag
        - git tag [tag-name]
        - git tag [tag-name] [commit]
        - git tag -d [tag]


##### remote repository
    * remote cmds
        - git fetch [remote]
        - git remote -v
        - git remote show [remote]
        - git remote add [shortname] [url]
        - git pull [remote] [branch]
        - git push [remote] [branch]


##### more information
    * git show
        - git show [tag]
        - git show [commit]
        - git show --name-only [commit]
        - git show [commit]:[file]
    * git diff
        - git diff
        - git diff HEAD
        - git diff --cached [file]
    * git log
        - git log --graph --pretty=oneline --abbrev-commit


##### redo & rollback
    * checkout
        - git checkout [file]
        - git checkout [commit] [file]
        - git checkout .
    * reset
        - git reset [file]
        - git reset --hard [commit]
        - git reset --keep [commit]
    * revert
        - git revert [commit]


##### 分支管理策略
    1. 主分支，代码只有一个主分支，所以正式版都在主分支上发布
    2. 开发分支develop，主分支只用来发布重大版本，日常开发在develop分支；发布时，在master分支上对develop分支进行合并
        - git checkout master
        - git merge --no-ff dev
    3. 临时分支
        3.1. 功能feature分支,功能分支的名字可以采用feature_x，使用完后应删除
            - git checkout -b feature-x dev
            - git checkout dev
            - git merge --no-ff feature-x
            - git branch -d feature-x
        3.2. 预发布release分支
        3.3. 修补bugfix分支


