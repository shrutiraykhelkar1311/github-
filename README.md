Git:-
Git is a distributed version control system that helps you track changes in your code.	
open-source distributed version control system. 
Version Control System is a tools that helps to track changes in code Git is a Version Control System. 


It is:
#popular
#free & Open Source
#fast & scalable
git helps is tracking the history and collabrate.

 
Feature of git 
Scalabiliy
Security 
Speed 
Open source

GitHub 
GitHub is a website where you can host and collaborate on Git repositories.
GitHub is a web-based platform that provides hosting for Git repositories and offers collaboration features for developers. 
It's a popular place for open-source projects and code sharing.
distributed version control and source code management (SCM)
 
Local = file on our laptop or pc
Remote=files on github


Git configure : 
 Git configuring is about setting up your personal information and customizing Git settings.

 Types of configure:
                                 1)global 
                                 2)local

Basic Command:-
git config --global user.name "My Name"
git config --global user.email "someone@email.com"
git config --list
	

Clone - Cloning a repository on our local machine(to make duplicate)
Cloning in Git creates a local copy of a repository on your machine .
(github varun apan project ,repo jya create kelelya astat tya vs code la copy or vs code vr ghenya sathi apan https or ssh chya link chya help ne copy karu shakto )

#Clone & Status
 

 git clone <- some link ->
Steps:-
Step 1: Open GitHub and navigate to the main page of the repository.
Step 2: Under the repository name, click on Clone or download.
Step 3: Select the Clone with HTTPs section and copy the clone URL for the repository. For the empty repository, you can copy the repository page URL from your browser and skip to next step.
Step 4: Open Git Bash and change the current working directory to your desired location where you want to create the local copy of the repository.
Step 5: Use the git clone command with repository URL to make a copy of the remote repository. 

 

Git clone branch:-
$ git clone -b <Branch name><Repository URL> 


Cloning a Repository into a Specific Local Folder
Git allows cloning the repository into a specific directory without switching to that particular directory. You can specify that directory as the next command-line argument in git clone command



Apan jr vs code modify kele kahi tr te M ne show hota ani tya nantr jr apan git status check kel tr  tithe modified:   as show hot. 
Jevha jevha apan modified karto konti file tevha ti add and commit karavich lagte.



# status –
 displays the state of the code
Mostly, it is used to display the state between Git Add and Git commit command.
git status
	
 
Status when a file is deleted
1.	$ git rm < File Name>  

Change             /          new file
(modified)                   (untracked)

Add                        (staged)

Commit         (unchanged)
#untracked
new files that git doesn't yet track
#modified
changed
#staged
file is ready to be committed(add)
#unmodified
Unchanged(commit)



#Add & Commit
add – 	add 	commit
adds new or changed files in your working directory to the Git staging area.
git add <- file name ->



Add multiple file 
Git add .


 
commit –(take a screenshot)
 it is the record of change
git commit -m "some message"

PS C:\Users\Dell\Desktop\demo\pritam-> git commit -m "add new words"
[main dae24e2] add new words
 1 file changed, 19 insertions(+)
PS C:\Users\Dell\Desktop\demo\pritam-> git status	command run outpout
On branch main
Your branch is ahead of 'origin/main' by 2 commits.  (use "git push" to publish your local commits)
 Push command= (push on github)	     push
Remote                               local

Push- upload local repo content to remote repo
Git push origin main



Origin= github repo
Main=barnch
 


Init Command
init - used to create a new git repo
git init
git remote add origin <- link ->(add new github remote repo)
gitgit remote -v (to verify remote)
git branch (to check branch)
git branch -M main (to rename branch)
git push origin main
Work flow
Local git
Github repo                 clone	change 	add	commit	push
Git branch:-
 in  Git, a branch is a new/separate version of the main repository.
Branch Commands
git branch      (to check branch)
git branch  -M main     (to rename branch)
git checkout <- branch name ->      (to navigate) go to one branch to another branch
git checkout  -b <- new branch name ->       (to create new branch)
git branch  -d <- branch name ->     (to delete branch)


 


Suppose ek project madhe 3 person vegal vegal kam karty tr te 3 person own branch create kartil ani tya branch vr kam kartil ani nantr last la tya merge kartil
We can perform various operations on Git branches. 
The git branch command allows you to create, list, rename and delete branches. 
Many operations on branches are applied by git checkout and git merge command. 
So, the git branch is tightly integrated with the git checkout and git merge commands

Github che content purn local madhe gheun yenya sathi pull command used kartat	
 
Merging Code
Way 1
git diff <- branch name->     (to compare commits, branches, files & more)
git merge <- branch name->   (to merge 2 branches)

Way 2
Using GitHub 
Create a PR(pull request)= 
  Pull request= It lets you tell other changes you’ve pushed to a branch in a repository on GitHub. 
For merge we create a pull request.
Pull command :-
Used to fetch and download content from a remote repo and immediately update the local repo to match that content

Resolving merge conflicts 
An evnet that takes place when git is unable to automatically resolve difference in code
Between two commits.
2 branch jr merge kele tr git la samjat nhi konte gheyche tya sathi manually aplyala resolve karav lagat

 
Undoing Changes(undo karne)
Case 1: staged changes(add zalet pn commit nhi zale)g
git reset <- file name ->git reset
 
Case 2: commited changes (for one commit)
git reset HEAD~1


 

HEAD~1 means a je pn commits ahet aplya javal te store karun internally git madhe .hya madhe je last commit ahe latest commit apan jyacha screenshot gheun thevla ahe tyach bydefult nav he HEAD . HEAD~1 mhnje head la reset kar 1 step











Case 3: commited changes (for many commits)
git reset <- commit hash ->




 
git reset --hard <- commit hash ->(all change reset on both)


 
Fork 
A fork is new repository that shares code and visibility setting with the original “upstream “repository
Fork is rough copy
 

Fork mhnje github chya dusryachya account varun project copy karun ek frok file create karne .ani tya project madhe apan sagale changes karu shakto





	






