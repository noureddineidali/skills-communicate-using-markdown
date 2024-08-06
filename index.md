# learning how to communicate using Markdown
I tried to use git and GitHub in the command line to complete this exercise  
These are the steps I used to do that 

1. First I cloned the the repository using the command `git clone https://github.com/noureddineidali/skills-communicate-using-markdown.git`  
> I'am already logged in with my GitHub account

2. Then I used `git fetch origin` to get the up-to-date information about the remote branches

3. I then checked out the branch start-markdown from the remote repo to the local repo using `git checkout -b start-markdown origin/start-markdown`
> In this branch the authors provided an empty file **index.md** which is the current file I am editing right now

4. After I made changes to the index.md file, I staged the changes for the next commit using `git add index.md` 

5. I commit the changes using `git commit indext.md -c "I described the steps I used to solve the exercice"` 

6. all I had to do now was to push the changes to the remote repo using `git push `
> in this step I encoutered an error, which was due to the fact that I cloned the repo using HTTPS, so i should have cloned the repo using SSH to make things simpler 

7. To fix this problem I used the command `git remote set-url origin git@github.com:noureddineidali/skills-communicate-using-markdown.git`  this comand allows me update the remote URL to use SSH
> N.B: I already had my own SSH key created before. 

8. Now running the command `git push` returns no errors, so my changes are pushed to the remote repository 

`  this comand allows me update the remote URL to use SSH
> N.B: I already had my own SSH key created before. 

8. Now running the command `git push` returns no errors, so my changes are pushed to the remote repository 


