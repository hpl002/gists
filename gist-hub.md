### Prelude
 While the git cli is expansive, it does not support creating new remote repositories directly from the terminal. 
 Ref: [forum post](https://github.community/t/creating-a-new-remote-repo-from-command-line/286) 

We can however use [hub](https://github.com/github/hub) to solve this slight annoyance..
___
 1. Install hub via your preferred package manager, instructions [here](https://github.com/github/hub#installation)

2. Initialize a new git repo locally
    ``` bash 
        cd 
        mkdir my-new-repo; 
        cd my-new-repo
        git init
    ``` 
3. add some content, stage file and commit
    ``` bash 
        touch yello.md        
        git add -A
        git commit . -m "init"
    ``` 
4. create new repo on remote
    ``` bash 
     hub create #This will create a new repository on remote with name: my-new-repo 
    git push --set-upstream origin master #push to remote
    ``` 

> Head over to github and check out your new repo: https://github.com

Cheers!

