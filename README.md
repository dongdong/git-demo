### Git cmd demo


##### basic cmds
    * information:
        - git status
        - git config --list
        - git config -e
        - git log
        - git reflog
        - git log --graph --pretty=oneline --abbrev-commit
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







