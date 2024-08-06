# learning how to communicate using Markdown
**I tried to use git and GitHub in the command line to complete this exercise.   
These are the steps I used to do that:**

1. Cloning the Repository:
```bash
git clone https://github.com/noureddineidali/skills-communicate-using-markdown.git
```  
> I'am already logged in with my GitHub account.

2. Fetching Remote Branches:
```bash
git fetch origin
```
> This command updates my local repository with the up-to-date information about the remote branches.

3. Checking Out the Branch start-markdown: 
```bash
git checkout -b start-markdown origin/start-markdown
```
> In this branch the authors provided an empty file **index.md**, which is the current file I am editing right now.

4. Making Changes:
> After I made changes to the **index.md** file, I staged the changes for the next commit using:
```bash
git add index.md
``` 

5. Committing Changes:
```bash
git commit indext.md -c "I described the steps I used to solve the exercice"
``` 

6. Pushing Changes:
> I tried to push the changes to the remote repository using:
```bash
git push
```
> In this step, I encountered an error because I cloned the repo using HTTPS. I should have cloned the repo using SSH to simplify authentication.

7. Fixing the Push Error:
```bash
git remote set-url origin git@github.com:noureddineidali/skills-communicate-using-markdown.git
```  
> This command updates the remote URL to use SSH.  
> Note: I already had my own SSH key created before.

8. Pushing Again:
```bash
git push
```
> This command pushes my changes to the remote repository without any errors.


9. Creating a Pull Request:
> The final step is to do a pull request and merge the start-markdown branch to the main branch.  
> The pull request and merging the branches could be done on the GitHub website, but I decided to open the pull request in CLI using:
```bash
gh pr create --base main --head start-markdown --title "getting started with markdown" --body "in the **index.md** file I added some steps I used to solve the exercise using git commands and I tried to do everything from cloning the repo, editing the file, pushing the changes, and also creating the pull request using **the command line interface**."
```

10. Merging the Pull Request:  
>The merge of the start-markdown branch to the main branch is done on the GitHub website.



--------


author: Nouredine Idali

date: 06/08/2024