# CS-AlliedBranches
GIT Lab Repository of all allied Branches of CS - DS, AI/ML, Design

First Change - Created 3 sub-folders for 3 different branches i.e for DS, AI/ML, Design. 

Setup commands -
1. ssh-keygen -t ed25519 -C "abc@gmail.com"
2. eval "$(ssh-agent -s)"
3. ssh-add ~/.ssh/id_ed25519
4. cat ~/.ssh/id_ed25519.pub
**Program 1 - 
Commands list - mkdir, cd, touch
1. git init
2. git status
3. git add .
4. git commit -m "a.c file created"
5. git log**

atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046$ mkdir folder1
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046$ cd folder1
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git init
Initialized empty Git repository in /home/atme/ci046/folder1/.git/
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ touch a.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	a.c

nothing added to commit but untracked files present (use "git add" to track)
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git add a.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   a.c

atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git commit -m "a.c file created"
[master (root-commit) f844b3a] a.txt created
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 a.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git status
On branch master
nothing to commit, working tree clean
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git log
commit f844b3a6b230221cad329708412443beb0d48a37 (HEAD -> master)
Author: Your <you@example.com>
Date:   Thu Jan 11 15:31:23 2024 +0530

    a.c file created

**Program 2 - ** Program 1 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log) + git branch, git branch feature, git checkout feature, git merge feature
Run program 1 and then run these commands - 

atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
* master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch feature
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
  feature
* master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git checkout feature
Switched to branch 'feature'
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
* feature
  master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ touch b.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git add .
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git commit -m "b.c is created "
[feature 2df2971] a.c is created
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 b.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git checkout master
Switched to branch 'master'
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
  feature
* master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ ls
a.c  
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git merge feature
Updating bfe24a8..2df2971
Fast-forward
  b.c | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 a.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ ls
a.c  b.c

**Program 3 - ** Program 1 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log) + git branch, git branch feature, git checkout feature, git stash save, git stash pop
Run program 1 and then run these commands - 
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
* master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch feature
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
  feature
* master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git checkout feature
Switched to branch 'feature'
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
* feature
  master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ touch b.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git add .
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git stash save


atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git checkout master
Switched to branch 'master'
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git branch
  feature
* master
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ ls
a.c  
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git stash pop

atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ ls
a.c  b.c

**Program 4 - ** Program 1 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log) + git clone, git branch, git branch feature, git checkout feature, git merge feature

atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046$ mkdir folder1
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046$ cd folder1 
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git clone https://github.com/Ponnanna-17/CS-AlliedBranches.git
Cloning into 'CS-AlliedBranches'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 1), reused 3 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), done.
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ ls
CS-AlliedBranches
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ cd CS-AlliedBranches/
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1/CS-AlliedBranches$ touch r.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1/CS-AlliedBranches$ git add .
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1/CS-AlliedBranches$ git commit -m "r.c is created"
[main 3a145ef] r.c is created
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 r.c
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1/CS-AlliedBranches$ git log
commit 3a145efff9af77c5df9d9ddf67a39248351e6bb4 (HEAD -> main)
Author: Your <you@example.com>
Date:   Thu Jan 11 15:43:08 2024 +0530

    r.c is created

commit 5942fcbf42db0c63d369381ce4d9e169400a7a44 (origin/main, origin/HEAD)
Author: ubuntu <ubuntu@ubuntu2.myguest.virtualbox.org>
Date:   Sat Nov 11 22:40:00 2023 +0530

    Commit No.one

commit 0b9a8d143787e41e936b5f464cb9178944a0de09
Author: Arjungs1524 <arjungs15@gmail.com>
Date:   Sat Nov 11 22:32:39 2023 +0530

    Initial commit

Program 5 -  Program 4 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log, git clone, git branch, git branch feature, git checkout feature, git merge feature) + git rebase

Program 6 - Program 4 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log, git clone, git branch, git branch feature, git checkout feature) + git merge feature 

**Program 7 -  **Program 1 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log) + git tag, git tag v1.0
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git tag
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git tag v1.0
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git tag
v1.0
**Program 8 - ** Program 4 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log, git clone, git branch, git branch feature, git checkout feature, git merge feature) + git cherry-pick 

**Program 9 - ** Program 1 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log) + git show f844b3a6b230221cad329708412443beb0d48a37
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git log
commit f844b3a6b230221cad329708412443beb0d48a37 (HEAD -> master, tag: v1.0)
Author: Your <you@example.com>
Date:   Thu Jan 11 15:31:23 2024 +0530

    a.c file created
atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git show f844b3a6b230221cad329708412443beb0d48a37
commit f844b3a6b230221cad329708412443beb0d48a37 (HEAD -> master, tag: v1.0, tag: v1)
Author: Your <you@example.com>
Date:   Thu Jan 11 15:31:23 2024 +0530

    a.c file created

diff --git a/a.c b/a.c
new file mode 100644
index 0000000..e69de29
Program 10 -  Program 4 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log, git clone, git branch, git branch feature, git checkout feature, git merge feature) + git log --author="name"
Program 11 -  Program 1 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log) + git log -2 or git log -5

repeat the below 3 commands  5 or 6 times for different file names and commit messages. 
i) atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ touch g.c
ii)atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git add .
iii) atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git commit -m "g.c file is created"
[master bfe24a8] g.c is created
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 g.c

 atme@atme-HP-280-Pro-G6-Microtower-PC:~/ci046/folder1$ git log -2 or git log -5
Program 12 -  Program 4 commands ( mkdir, cd, touch. git init, git status, git add ., git commit -m "a.c file created", git log, git clone, git branch, git branch feature, git checkout feature, git merge feature) + git reset
