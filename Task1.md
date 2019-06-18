# Task 1: Mastering Git

[TOC]

### What is VCS? Why is it important?

#### What is VCS?

​	Version Control Systems is one of the most important tools for any project. It is a category of software tool that help a software team manage changes to the source code over time. This system is also called as Revision Control or Source Code Management. It allows the user to manage changes in the documents, computer programs, websites etc.  The system keeps track of every modification to the code  in a special kind of database. These modifications or revisions can then be compared, restored and merged using this system.

#### Why do we need Version Control?

​	VCS can be used for various reasons like maintaining multiple versions of a product, reverting back certain changes that are brought about in the code, trying to back up very old or lost codes,bringing about changes in others codes or letting other people changing your codes, experimenting with the code without bringing about changes in  the working code, etc.

Some benifits of using VCS are :

1. Version tracking andbranching: Every change that is madeis persisted in the system. Thus it compares files, identifies changes andmerges the changes.
2. Tagging: This systemallows users to tag a project so that one can referit back later whenever required.
3. Restoring PreviousVersion: The system restores previousversion of any file. This feature is very helpful when the user accidentallydeletes a code or performs changes which break existing code.
4. Collaboration: Thesystem allows multiple people to work on same files or folders simultaneously.The system then merges all the changes to one common revision.
5. Audit: Since all the changes are maintained in the system it is easierto audit the file.
6. Easy Integration withIDE: The system can be integrated withIDE's very easily. Thus the user can use the same tool he is working on.  

***

### How to clone a Git repository?

#### Why do we need to clone a repository?

​	When a new repository is created on GitHub, the project is stored on a  remote location. Cloning is done so that the user can sync between the local location on the computer and remote location of the project. This is also used when the user wants projects done by 2 individuals to get merged so that he gets a single project.

In Git, this can be done through a Git Clone. It basically

1. Initializes a local repository
2. Adds the remote URL to the local repository
3. Pulls the repository onto the computer.

#### To clone the repository:

1. On GitHub, navigate to the repository file which you want to clone. 
2. Under the repository name, click ==**Clone or download**==.
3. Copy the URL which is given there. 
4. Open **Git Bash**.
5. Change the directory in Git Bash to the location where you want the cloned directory to be made.
6. Type ==**git clone (paste URL)**==.
7. Press **Enter**.


> Example: git clone https://github.com/Bhoomika73/testit.git

***

### How to pull/push to remote repository?

The **push** command sends changes to the master branch of your remote repository.

#### To Push commits made on the remote repository:

1. Go to **Git Bash**.
2. Type ==**git push -u (remote) (branch)**==
3. Press **Enter**.

The  **Push** command takes two arguments:

- A remote name,     for example: origin
- A branch name,     for example: master

> Example: git push -u origin master

#### To pull from a Git Repository:

1. Go to **Git Bash**.
2. Type ==**git pull**==
3. Press **Enter**.

The **Pull** Command is used to fetch and merge changes on the remote server to the required working directory

***

### How to check the status of the repository?

#### Why do we need to check the status of the repository?

​	The command is used to check the status of the repository and report if there is anything to commit and records if any changes have to be done to the project. This command keeps monitoring the states of both the working directory and the repository. 

#### To check the status of the repository:

1. Go to **Git Bash**.
2. Type ==**git status**==
3. Press **Enter**. 

***

### How to create and switch to a branch?

#### To create a new branch:

1. First create a branch locally.
2. For this go to **Git Bash**.
3. Type ==**git branch (branch name)**== 
4. Press **Enter**.

#### To switch to the branch:

1. Type ==**git checkout -b (branch-name)**==.
2. Type ==**push (remote)(branch-name)**==.
3. Press **Enter**.

***

### How to connect to a remote a repository?

To add a new remote to the repository 

1. Go to **Git Bash**.
2. Type ==**git remote add (remote name)(remote URL)**==.
3. Press **Enter**.

The **git remote add** command takes two arguments:

- A remote name, for example: origin
- A remote URL, for example: https://github.com/user/repo.git

>Example: git remote add origin https://github.com/user/repo.git

***

### How to merge two branch?

#### When do we merge 2 branches?

​	If a situation arises when the working project is in branch "A". Suppose the programmer makes changes to this branch and saves it in branch “B” and now wants to get only one branch then he must merge the 2 branches.

#### To merge 2 branches:

1. Go to **Git Bash**.
2. Type ==**git checkout A**== and press **Enter** to switch to branch A.
3. Type ==**git merge B**== and press **Enter** to merge all changes from branch B into branch A.
4. Type ==**git commit -A**== and press **Enter** to commit all the changes.

***

### How to resolve merge conflicts?

#### When does merge conflicts occur?

​	Merge conflicts occur when competing changes are made to the same line of a file, or when one person edits a file and another person deletes the same file. The most common situation is when the exact same line of a file are edited in conflicting ways.

#### To resolve merge conflicts:

1. First check if there is any merge conflicts in the file. 
2. For this type ==**git status**== and press **Enter** . By this the user will get to know if there is any merge conflicts and which is the line that has the merge conflict.
3. Solve the merge conflict by editing the particular lines. For this, open the file in the editor and make the necessary modifications.

***

### How to commit changes?

1. First resolve all the merge conflicts and do all the necessary changes.
2. Open **Git Bash**.
3. Then type ==**git commit -m "(comment)" (file name)**==.
4. Then press **Enter**.

***

### How to stash changes?

​	Once the changes are done in the project, the user either has to commit these changes or lose them by switching to the other commit. If he does not want to do either of these options, then he can do Stashing. For this,

1. Type ==**git stash save (filename)**==.
2. Press **Enter**.

***

