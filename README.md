# repu
C:\Users\Neer>cd C:/

C:\>cd neer

C:\neer>cd gitlab

C:\neer\gitlab>mkdir expr1

C:\neer\gitlab>git init
Initialized empty Git repository in C:/neer/gitlab/.git/

C:\neer\gitlab>cd expr1

C:\neer\gitlab\expr1>git config --global --list
user.email=neerpandey$@gmail.com
user.name=neerpandey4

C:\neer\gitlab\expr1>git clone https://github.com/neerpandey4/repo2.git
Cloning into 'repo2'...
remote: Enumerating objects: 18, done.
remote: Counting objects: 100% (18/18), done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 18 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (18/18), 5.32 KiB | 681.00 KiB/s, done.

C:\neer\gitlab\expr1>cd repo2

C:\neer\gitlab\expr1\repo2>git fetch origin
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 920 bytes | 27.00 KiB/s, done.
From https://github.com/neerpandey4/repo2
   c9fbb6a..7645031  main       -> origin/main

C:\neer\gitlab\expr1\repo2>git rebase origin/main
Successfully rebased and updated refs/heads/main.

C:\neer\gitlab\expr1\repo2>git add README.md

C:\neer\gitlab\expr1\repo2>git fetch origin

C:\neer\gitlab\expr1\repo2>git rebase origin/main
error: cannot rebase: Your index contains uncommitted changes.
error: Please commit or stash them.

C:\neer\gitlab\expr1\repo2>git commit -m "modified"
[main 3cfa367] modified
 1 file changed, 1 insertion(+)

C:\neer\gitlab\expr1\repo2>git fetch origin
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 929 bytes | 20.00 KiB/s, done.
From https://github.com/neerpandey4/repo2
   7645031..2477d3c  main       -> origin/main

C:\neer\gitlab\expr1\repo2>git rebase origin/main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 3cfa367... modified
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply 3cfa367... modified

C:\neer\gitlab\expr1\repo2>git add README.md

C:\neer\gitlab\expr1\repo2>git rebase --continue
[detached HEAD 5a983f9] modified
 1 file changed, 1 insertion(+)
Successfully rebased and updated refs/heads/main.

C:\neer\gitlab\expr1\repo2>git add README.md

C:\neer\gitlab\expr1\repo2>git commit -m "Read me"
[main f5aee49] Read me
 1 file changed, 1 insertion(+)

C:\neer\gitlab\expr1\repo2>git stash save "my file save"
No local changes to save

C:\neer\gitlab\expr1\repo2>git checkout -b targetbranch
Switched to a new branch 'targetbranch'

C:\neer\gitlab\expr1\repo2>git stash apply
No stash entries found.

C:\neer\gitlab\expr1\repo2>git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

C:\neer\gitlab\expr1\repo2>git checkout -b "tb"
Switched to a new branch 'tb'

C:\neer\gitlab\expr1\repo2>git stash apply
No stash entries found.

C:\neer\gitlab\expr1\repo2>git stash save "file"
No local changes to save

C:\neer\gitlab\expr1\repo2>git stash apply
No stash entries found.

C:\neer\gitlab\expr1\repo2>
