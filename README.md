# Cloning
(cloning remote repo to reach local repo)
1. (base) PS D:\Baraka> git clone https://github.com/tanjida100/New-project.git
Cloning into 'New-project'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.
## Go to that cloning file:
2. PS D:\Baraka> cd New-project

3. (base) PS D:\Baraka\New-project> ls


    Directory: D:\Baraka\New-project


|Mode|                     LastWriteTime|         Length Name|

|----|                 -------------|         ------ ----|

|-a----        | 7/30/2026   3:53 PM |            20 Docker1.txt|

|-a----  |       7/30/2026   3:53 PM |            48 README.md|

4. ### Personal access token
go to git account -> setting -> Developer->personal access token
then generate your token.
5. __use gitbash when create file (touch text1.txt)__
6. __Add to  git__
(base) PS D:\Baraka\tanjida\notes-2> git add text1.txt
(base) PS D:\Baraka\tanjida\notes-2> git commit -m "added more information"
[master 0f55a6f] added more information
 2 files changed, 11 insertions(+), 5 deletions(-)

7. __if chng anything after already push something in git then type git push__
(base) PS D:\Baraka\tanjida\notes-2> git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 505 bytes | 505.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:tanjida100/git_learning2.git
   01beb74..0f55a6f  master -> master
(base) PS D:\Baraka\tanjida\notes-2> git log --oneline
0f55a6f (HEAD -> master, origin/master) added more information
01beb74 added infor
d8de843 (gitlearning/master) leaning github2
8. __If change anything from github acount then pull all that changer in desktop use git pull__
(base) PS D:\Baraka\tanjida\notes-2> git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1002 bytes | 5.00 KiB/s, done.
From github.com:tanjida100/git_learning2
   0f55a6f..fb6281f  master     -> origin/master
Updating 0f55a6f..fb6281f
Fast-forward
 text1.txt | 1 +
 1 file changed, 1 insertion(+)
9. __see all commit in omneline ,helps to shortage the key value__
(base) PS D:\Baraka\tanjida\notes-2> git log --oneline
fb6281f (HEAD -> master, origin/master, origin/HEAD) added warning masseg
0f55a6f added more information
01beb74 added infor
d8de843 (gitlearning/master) leaning github2