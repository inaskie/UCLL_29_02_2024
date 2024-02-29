Microsoft Windows [Version 10.0.19045.4046]
(c) Microsoft Corporation. Alle rechten voorbehouden.

C:\WINDOWS\system32>ls
'ls' is not recognized as an internal or external command,
operable program or batch file.

C:\WINDOWS\system32>cd ..

C:\Windows>cd ..

C:\>mkdir workspace

C:\>cd workspace

C:\workspace>mkdir gitworkshop

C:\workspace>cd gitworkshop

C:\workspace\gitworkshop>echo "# UCLL_29_02_2024" >> README.md

C:\workspace\gitworkshop>git init
Initialized empty Git repository in C:/workspace/gitworkshop/.git/

C:\workspace\gitworkshop>git add README.md

C:\workspace\gitworkshop>git commit -m "first commit"
[master (root-commit) ee836fd] first commit
 Committer: Inas Mezouri <r0987139@ucll.be>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 README.md

C:\workspace\gitworkshop>git branch -M main

C:\workspace\gitworkshop>git remote add origin https://github.com/inaskie/UCLL_29_02_2024.git

C:\workspace\gitworkshop>git push -u origin main
info: please complete authentication in your browser...
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 235 bytes | 235.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/inaskie/UCLL_29_02_2024.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

C:\workspace\gitworkshop>git add README.md

C:\workspace\gitworkshop>git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

C:\workspace\gitworkshop>git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

C:\workspace\gitworkshop>git add README.md

C:\workspace\gitworkshop>git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


C:\workspace\gitworkshop>git init
Reinitialized existing Git repository in C:/workspace/gitworkshop/.git/

C:\workspace\gitworkshop>git add README.md

C:\workspace\gitworkshop>git commit -m "first commit"
[main 0786387] first commit
 Committer: Inas Mezouri <r0987139@ucll.be>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 9 insertions(+)

C:\workspace\gitworkshop>git branch -M main

C:\workspace\gitworkshop>git remote add origin https://github.com/inaskie/UCLL_29_02_2024.git
error: remote origin already exists.

C:\workspace\gitworkshop>git add README.md

C:\workspace\gitworkshop>git commit README.md
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\workspace\gitworkshop>git push README.md
fatal: invalid gitfile format: README.md
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

C:\workspace\gitworkshop>git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 6 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 361 bytes | 361.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/inaskie/UCLL_29_02_2024.git
   ee836fd..0786387  main -> main

C:\workspace\gitworkshop>git push README.md
fatal: invalid gitfile format: README.md
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

C:\workspace\gitworkshop>git add README.md

C:\workspace\gitworkshop>git commit -m "first commit"
[main 33d3fb7] first commit
 Committer: Inas Mezouri <r0987139@ucll.be>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 4 insertions(+), 3 deletions(-)

C:\workspace\gitworkshop>git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\workspace\gitworkshop>git push -u origin main
To https://github.com/inaskie/UCLL_29_02_2024.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/inaskie/UCLL_29_02_2024.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

C:\workspace\gitworkshop>git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 1020 bytes | 92.00 KiB/s, done.
From https://github.com/inaskie/UCLL_29_02_2024
   0786387..6efa19e  main       -> origin/main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.

C:\workspace\gitworkshop>commit -m "second change"
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\workspace\gitworkshop>git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

C:\workspace\gitworkshop>git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

C:\workspace\gitworkshop>git commit -a
[main b3752a9] Merge branch 'main' of https://github.com/inaskie/UCLL_29_02_2024
 Committer: Inas Mezouri <r0987139@ucll.be>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author


C:\workspace\gitworkshop>git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 6 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 751 bytes | 375.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/inaskie/UCLL_29_02_2024.git
   6efa19e..b3752a9  main -> main

C:\workspace\gitworkshop>
