### Git cmd demo


##### on master branch
    * add README.md and first commit
    * basic git cmds:
        - git init
        - git config --list
        - git config -e
        - git status
        - git commit -m [message]
        - git log
        - git reflog
        - git reset --hard [commit]
        - git rm [file1] [file2] ...
        - git rm --cached [file]
        - git mv [file-original] [file-renamed]
        - git commit --amend -m [message]


##### on dev branch
    * git branch cmds:
        - git branch
        - git branch [branch-name]
        - git checkout [branch-name]
        - git checkout -b [branch-name]
        - git branch [branch-name] [commit]
        - git checkout -
    * remote branch
        - git branch -r
        - git branch --track [branch] [remote-branch]
        - git branch --set-upstream [branch] [remote-branch]
    * merge
        - git merge [branch]
        - git merge --no-ff [branch]
