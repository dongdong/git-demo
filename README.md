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
    * remote branch
        - git branch -r
        - git branch --track [branch] [remote-branch]
        - git branch --set-upstream [branch] [remote-branch]
    * branch merge
        - git merge [branch]
        - git merge --no-ff [branch]
