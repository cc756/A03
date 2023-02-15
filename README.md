# A03-cc756
## Git Tutorial
### Step 1-Install GIT
Download **GIT** for free from [here](https://git-scm.com).
### Step 2-Check GIT Installation
Open up a command shell and use the following commands:
```
git --version ###enter this line
git version X.Y.Z.osbrand.A ###this should be the return line
```
### Step 3-Introduce Yourself to GIT
GIT needs to get to know you, as you to are goin to be very comfy for the rest of your time working in the computer industry. It is also important for version control systems as commits from GIT use this information each time. Use the following commands:
```
###substitute your own information
git config --global user.name "cc756"
git config --global user.email "cc745@njit.edu"
```
> `global` will set the username and e-mail for every **repository** on your computer, remove it from the command to do it for just the current repository.
### Step 4-New Directory
Let's refresh our System Admin skills and make a new directory for our project.
```
mkdir projectName ###makes a new director called projectName
cd projectName ###change current working directory to projectName
```
### Step 5-Time to Intitialize
Let's initialize Git and create our first GIT repo. Git will keep track of changes to this folder for changes and keep track of it in a hidden folder.
```
git init
Intialized empty Git repository in /Users/user/projectName/.git/
```
Congratulations on creating your first local repo!
## GitHub Tutorial
### Step 1-Make Account
Go to [GitHub](github.com) and create an account for **GitHub**.
![Account Creation](https://www.w3schools.com/git/img_githup_sign_up.png)
### Step 2-Make Repository
Click plus button dropdown in the upper righthand corner of the site on the navigation bar. Click the button that says `New repository`.
![Repo Creation](https://www.w3schools.com/git/img_github_new_repo.png)
Fill in the info for your repository. This one is for a W3 Schools [tutorial](https://www.w3schools.com/git/git_remote_getstarted.asp?remote=github). We will be following that tutorial for the rest of this.
![Repo Info](https://www.w3schools.com/git/img_github_new_repo_create.png)
### Step 3-It's time to Push
Now the first time is going to be tough but we are going to **push** that repo we created in the GIT tutorial to your new GitHub account. Now breathe with me as we take our GitHub username and the GitHub repo name and combine into a URL like the one below.
> https://github.com/cc756/A03.git
Now we take this URL and breathe out as we head back to our command line.
```
git remote add origin https://github.com/cc756/A03.git
```
`git remote add origin URL` specifies that you are adding a **remote** repository, with the specified `URL`, as an `origin` to your local Git repo.
Okay it's time for that big push! I'll hold your hand if you need it as if this is your first time you will get a notification to authenticate.

**3**

**2**

**1**

**PUSH!**
```
git push --set-upstream origin master
Enumerating objects: 22, done.
Counting objects: 100% (22/22), done.
Delta compression using up to 16 threads
Compressing objects: 100% (22/22), done.
Writing objects: 100% (22/22), 92.96 KiB | 23.24 MiB/s, done.
Total 22 (delta 11), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (11/11), done.
To https://github.com/cc756/A03.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
```
### Step 5-Awwww, It's Connected
Go back to your repository on GitHub to see if the **merge** happened or if there was a **merge conflict**.
![Successful Push](https://www.w3schools.com/git/img_github_merged.png)

##Webstorm
1. Go to [JetBrains](https://www.jetbrains.com) and create an account
2. Apply for a student license to Webstorm
3. Wait for a while for JetBrains to email you back
4. Use the link in the email to activate your license
5. Download the standalone Webstorm or the JetBrains' Toolbox App and then download Webstorm within that
6. Open up Webstorm and be greeted by this great interface.
![User Interface](https://github.com/cc756/A03/blob/main/imageFolder/Click%20VCS.png)
7. Realize around this point you don't know what to do anymore
8. Authorize your GitHub account in Webstorm

![User Interface](https://github.com/cc756/A03/blob/main/imageFolder/Authorize.png)

9. Once authorized **clone** the repostiory you want
![User Interface](https://github.com/cc756/A03/blob/main/imageFolder/Clone.png)

## Glossary
**Branch**: a new/separate version of the main repository. Allows to developers to edit the code without effecting the main branch, allowwing for mulititasking among the teams.

**Clone**: `git clone` creates a local copy of a project that already exists remotely. The clone includes all the project's files, history, and branches.

**Commit**: `git commit` saves the snapshot to the project history and completes the change-tracking process. In short, a commit functions like taking a photo. Anything that's been staged with `git add` will become a part of the snapshot with `git commit`.

**Fetch**: allows users to download files and changes from the remote to their local repository. Generally good practice to run `git fetch` before you start

**GIT**: a version control system tracks the history of changes as people and teams collaborate on projects together. Unlike once popular centralized version control systems, distributed version control systems don't need a constant connection to a central repository. Git is the most popular distributed version control system. Also used to start commands when using Git directly from the command line

**Github**: a website that hosts Git repositories and provides developers with tools to ship better code through command line features, issues (threaded discussions), pull requests, code review, or the use of a collection of free and for-purchase apps in the GitHub Marketplace.

**Merge**: `git merge` joins two or more branches together and incorporates the changes from the named commits into the current branch the user is working in.

**Merge Conflict**: when two branches have commits that conflict with each other and you attempt to merge them, Git needs to decide which commits to actually use in the final merge. This is usually done automaticaly but sometimes Git needs your help.

**Push**: `git push` updates the remote repository with any commits made locally to a branch.

**Pull**: `git pull` updates the local line of development with updates from its remote counterpart. Developers use this command if a teammate has made commits to a branch on a remote, and they would like to reflect those changes in their local environment.

**Remote**: a repository that is hosted on a server that is accessible to all team members. Code hosting services such as Github can serve as storage for remote repositories.

**Repository**: a collection of files that are compiled together into a project, along with the commit/file revision history of that project

## References
<details><summary>Click for references</summary> 
<p>
  
  - [Jet Brains](https://www.jetbrains.com/help/webstorm/getting-started-with-webstorm.html) was going to use this more but ran out of time before I could get to it
  - [GitHub Docs](https://docs.github.com/en)
  - [W3 Schools Git Tutorial](https://www.w3schools.com/git/)
  - Past classes
  
</p>
</details>
