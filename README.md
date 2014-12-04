> git clone https://github.com/hhru/frontik.git hh_git_task2_without_frontik

Cloning into 'hh_git_task2_without_frontik'...

remote: Counting objects: 7596, done.

remote: Compressing objects: 100% (2502/2502), done.

remote: Total 7596 (delta 5103), reused 7509 (delta 5023)

Receiving objects: 100% (7596/7596), 1.72 MiB | 947.00 KiB/s, done.

Resolving deltas: 100% (5103/5103), done.

Checking connectivity... done.

> cd hh_git_task2_without_frontik

> git filter-branch --tree-filter "rm -f -r frontik"

Rewrite 445a2f8c85420bca45b3b8a76ec20c9153097635 (639/1177)error: duplicate parent c85af632b217d23c6d38f8b64c50aada6dba78eb ignored

Rewrite 4cbc4b91ff591b9f2372fa7714b50d16ba7e07ff (1177/1177)

Ref 'refs/heads/master' was rewritten

> git remote add sv https://github.com/svesipov/hh_git_task2_without_frontik

> git push sv master

Counting objects: 5229, done.

Delta compression using up to 4 threads.

Compressing objects: 100% (2446/2446), done.

Writing objects: 100% (5229/5229), 1.09 MiB | 448.00 KiB/s, done.

Total 5229 (delta 3157), reused 4048 (delta 2719)

To https://github.com/svesipov/hh_git_task2_without_frontik

[new branch]      master -> master
 
> cd ..
 
> git clone https://github.com/hhru/frontik hh_git_task2_with_frontik

Cloning into 'hh_git_task2_with_frontik'...

remote: Counting objects: 7596, done.

remote: Compressing objects: 100% (2502/2502), done.

remote: Total 7596 (delta 5103), reused 7509 (delta 5023)

Receiving objects: 100% (7596/7596), 1.72 MiB | 900.00 KiB/s, done.

Resolving deltas: 100% (5103/5103), done.

Checking connectivity... done.

> cd hh_git_task2_with_frontik/

> git filter-branch -f --tree-filter "ls -a | grep -v -xE 'frontik|\.|\.\.' | xargs rm -rf"

Rewrite 445a2f8c85420bca45b3b8a76ec20c9153097635 (639/1180)error: duplicate parent 12444114fde78b843285d819d461f1be211ca031 ignored

Rewrite 2a6d5bfdde263d6d007d7d467f909b4e94481ead (1180/1180)

Ref 'refs/heads/master' was rewritten

> git remote add sv https://github.com/svesipov/hh_git_task2_with_frontik

> git push sv master

Counting objects: 2920, done.

Delta compression using up to 4 threads.

Compressing objects: 100% (1355/1355), done.

Writing objects: 100% (2920/2920), 706.74 KiB | 0 bytes/s, done.

Total 2920 (delta 1276), reused 1263 (delta 1101)

To https://github.com/svesipov/hh_git_task2_with_frontik

[new branch]      master -> master
