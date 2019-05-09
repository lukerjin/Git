# Git questions & issues
### Difference between _Git Pull_ and _Git Clone_

`Git Clone`: When there is no repository in local, then download the repository from remote.  
`Git Pull`: When there is repository in local, if there is new __Commit__ in remote repository, then download and merge it the new __Commit__ with local file.  

### Fetch and merge all remote branches
`git branch -r | grep -v '\->' | while read remote;do git branch --track "${remote#origin/}" "$remote"; done`  
`git fetch --all`  `git remote update`  
`git pull --all` 

### To exit the commandline insert
Press ESC and then type :wq  

### How to make an existing branch track a remote branch?
`--set-upstream-to` + remote name  
`$ git branch --set-upstream-to origin/master`  

### Reference Sites
[book git-scm](https://book.git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)  
[How to fetch all Git branches](https://stackoverflow.com/questions/10312521/how-to-fetch-all-git-branches)  
