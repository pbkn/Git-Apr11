# Git-Apr11
Git Learn Session

GIT :

- IT is a distributed source version control system

control system- git mainly wokrs in content tracker 

version sytsem -> many developer make therir code changes in parallel 
at one specific point , you can make it for relesase ( version ) 


distributed version control system -> it can be used in local as well as remote 

GIT is open source 

-------------------------------------------------
GIT we have 3 stages 
------------------------
1. Working area 
2. Staggeing area 
3. Commit History 

---------------------------------------------------
Working area --> Stagging area -----> Commit History     -----> Github(remote)

Local Repository 
___________________________________________________
Hands on 
_________________________________________
Step1 : Create a empty repository in your local machine 
	git init 

Step 2: Create the file with source code 
	touch a.txt

Step 3: vi a.txt -> press insert button for insert mode to write the code 

Step 4: Go back to terminal-> esc+:+wq+enter

Step 5: after write the code -> check the status ( git status)
	the file will be in Working area 

Step 6: Move the file to stagging area ( git add .)

Step 7: After stagging , you need to commit(permenatly saved)
	git commit -m"file a.txt created and commit"

After commit will happen 

git create => 40 digit hashkey (checksum) with the help SHA alg 

Step 8: After commiting the file -> git log
----------------------------------------
Step 9: open the a.txt and adding some more source code 

Step 10:check the git status and git diff( working & stagging)

Step 11: add the file to satagging area ( git diff --stagged)

Step 12: open the a.txt and add contents 

Step 13: if the file not commited - git checkout -- .

Step 14: if the file commited -> git revert hashkey

Step 15: git reset --hard (hashkey-optional)

Step 16: go to Git apr 11 and delete a.txt manually
	 then it will be in working area -> git add . -> follow step 15

Step 17: go to Git apr 11 and delete using git rm filename 
	 then it will be in stagging area -> follow step 15
--------------------------------------------------------------------
Restricting the files
__________________________

Step 18: Open teh git bash

Step 19: create 3 files  ( a.png ,a.pdf.a.docx)

Step 20: check the git status(it will be in working area) 

Step 21:create .gitignore and (restrict the file using *.pdf)

Step 22:git status -> it will restrict and them git add . to the neccessary file 
------------------------------------------------------------------------------Tag 
-----------
Syntax for creating the file 
---------------------------
Light weight tag:
git tag tagname 

Annotated tag:
git tag -a tagname -m"message"
--------------------------------
Syntax for show the tag name :
------------------------------
git show tagname 
git show --tags

To push to remote repository 
--------------------------------
git push origin tagname 
git push --tag
git push origin --tags

To delete the tagname 
-----------------------
git tag -d tagname 
git tag --delete tagname 

git push origin -d tagname 
----------------------------------------------------
Branching and Merging 
___________________
To check the list of branch 
git branch 

To create the branch 
git branch brnachname 

To checkout to particular branch 
git checkout branchname 

git checkout -b branchname

To merge the branch 
git merge branchname 

To delete the branch name 
git -d branchname 


Step 1: create the branch called develop 
Step 2: switch to your branch 
Step 3: do the changes 
Step 4: commit 
Step 5: checkout to master
Step 6: Merge 
---------------------------
Pushing to remote repository 

Step 1: In github create new repository 
Step 2: In git bash -> git clone https://github.com/admininstrator_name/reponame.git foldername 

step3: DO stagging and commit 
Step 4: git push origin master to push the files to remote repo
----------------------------------------------------------------------- 
