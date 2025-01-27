# Learn git

For older notes: [https://sahilrajput03.github.io/Git_and_GitHub.html](https://sahilrajput03.github.io/Git_and_GitHub.html)

## show all branch

`git branch`: Prints all branches and \* indicated is the current branch.

## Creating new branch

`git branch test` : will make `test` named branch.

`git branch somebranch SourceBranchHere` will make `somebranch` named branch.

## switching to other branch

`git checkout branchName`

## logs

`git log`

## Remove a .env file from entire history of the repo

[Click here](https://daily-dev-tips.com/posts/removing-a-env-file-from-git-history/)

## What is .gitkeep

![image](https://user-images.githubusercontent.com/31458531/202268566-11a8a084-d48b-4eff-be46-83076c0d67c1.png)

## this is how you include a folder with a single file .gitkeep but ignore its other contens for personal usage for each team member

![image](https://user-images.githubusercontent.com/31458531/202270076-b8861f4d-515f-48a4-b837-28170166b62e.png)

## `git pull` vs. `git pull origin` vs. `git pull origin main`

- You're working on a branch called `SD-499` which was checked out from main.
- Now main branch on the remote repository is updated.
- Now you do `git pull` or `git pull origin`, this will only fetch and merge all remote branches to their respective local branches which set set t to tracked.
- SO, now you need to merge `main` branch into your current branch either by doing `git merge main` or you can do it by `git pull origin main` as both will do same thing. **Why?** Ans. Because `git pull origin main` will pull update local main branch first and second it will merge `main` branch to your `currently checkout branch`. BECAUSE `git pull` = `git fetch` + `git merge branch`. Source: [Atlassian](https://www.atlassian.com/git/tutorials/syncing/git-pull), [Git-scm](https://git-scm.com/docs/git-pull)

![image](https://user-images.githubusercontent.com/31458531/203025083-653be64f-ee49-41ad-9cd0-1c7da45faa57.png)

## View the commit diff of merged commit?

That can work actually.

![image](https://user-images.githubusercontent.com/31458531/206040759-0be29cd9-2033-40ba-bbb1-cc1fffc8a7c2.png)

##  ♥💕❤😘 You can literally move your `.git` folder any where

Yes, it sounds quite unbelievable but its quite magical how it does work actually. **Amazing Linus Torwald.**
