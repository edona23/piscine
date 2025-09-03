c4r6s3% pwd
/home/ehunda/c00/ex01
c4r6s3% cd exo2
cd: no such file or directory: exo2
c4r6s3% cd ex02
cd: no such file or directory: ex02
c4r6s3% cd ../
c4r6s3% cd ex02/
c4r6s3% cat test3
c4r6s3% a
zsh: command not found: a
c4r6s3% nano test3
c4r6s3% pwd   
/home/ehunda/c00/ex02
c4r6s3% cat test3
c4r6s3% chmod 777
chmod: missing operand after ‘777’
Try 'chmod --help' for more information.
c4r6s3% chmod 777 test3
c4r6s3% ls -ld test3
-rwxrwxrwx 1 ehunda 2025_london 2 Sep  3 15:41 test3
c4r6s3% ls  -l test2
total 0
c4r6s3% touch -d "2025/06/01 23:44" test3
c4r6s3% chmod -R 404 test3
c4r6s3% ls -ld test3
-r-----r-- 1 ehunda 2025_london 2 Jun  1 23:44 test3
c4r6s3% pwd
/home/ehunda/c00/ex02
c4r6s3% cat > test3
zsh: permission denied: test3
c4r6s3% cat > test4
ad
c4r6s3% ls -l test4
-rw-r--r-- 1 ehunda 2025_london 3 Sep  3 15:44 test4
c4r6s3% touch -d "2025/06/01 23:43" test4
c4r6s3% chmod -R 644 test4
c4r6s3% ls -l test4
-rw-r--r-- 1 ehunda 2025_london 3 Jun  1 23:43 test4
c4r6s3% chmod -R 641 test4
c4r6s3% ls -l test4
-rw-r----x 1 ehunda 2025_london 3 Jun  1 23:43 test4
c4r6s3% chmod -R 777
chmod: missing operand after ‘777’
Try 'chmod --help' for more information.
c4r6s3% chmod -R 777 test4
c4r6s3% chmod -R 641 test4
c4r6s3% ls -l test4 
-rw-r----x 1 ehunda 2025_london 2 Sep  3 15:47 test4
c4r6s3% chmod -R 777 test4
c4r6s3% touch -d "2025/06/01 23:43" test4
c4r6s3% ls -l test4
-rwxrwxrwx 1 ehunda 2025_london 2 Jun  1 23:43 test4
c4r6s3% chmod -R 641 test4
c4r6s3% ls -l test4
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
c4r6s3% 
c4r6s3% pwd
/home/ehunda/c00/ex02
c4r6s3% cat > test5 
a
c4r6s3% touch -D "2025/06/01 23:44" test5
touch: invalid option -- 'D'
Try 'touch --help' for more information.
c4r6s3% touch -d "2025/06/01 23:44" test5

c4r6s3% ls -l test5
-rw-r--r-- 1 ehunda 2025_london 2 Jun  1 23:44 test5
c4r6s3% nano test5
c4r6s3% ls -l test5
-rw-r--r-- 1 ehunda 2025_london 1 Sep  3 15:54 test5
c4r6s3% cat test5

c4r6s3% touch -d "2025/06/01 23:44" test5
c4r6s3% chmod -R 404 test5
c4r6s3% ls -l test5
-r-----r-- 1 ehunda 2025_london 1 Jun  1 23:44 test5
c4r6s3% 
c4r6s3% pwd
/home/ehunda/c00/ex02
c4r6s3% ln -s ex02/ test6
c4r6s3% ls -l
total 16
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwx--xr-- 1 ehunda 2025_london 4 Sep  3 15:09 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-r-----r-- 1 ehunda 2025_london 2 Jun  1 23:44 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-r-----r-- 1 ehunda 2025_london 1 Jun  1 23:44 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Sep  3 15:58 test6 -> ex02/
c4r6s3% chmod -R 777 test1
c4r6s3% touch -d "2025-06-01 21:46" test1
c4r6s3% ls -l
total 16
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwxrwxrwx 1 ehunda 2025_london 4 Jun  1 21:46 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-r-----r-- 1 ehunda 2025_london 2 Jun  1 23:44 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-r-----r-- 1 ehunda 2025_london 1 Jun  1 23:44 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Sep  3 15:58 test6 -> ex02/
c4r6s3% chmod -R 714 test1
c4r6s3% touch -h -t "2025/06/01 22:20" test6
touch: invalid date format ‘2025/06/01 22:20’
c4r6s3% touch -h -d "2025/06/01 22:20" test6
c4r6s3% ls -l test6
lrwxrwxrwx 1 ehunda 2025_london 5 Jun  1 22:20 test6 -> ex02/
c4r6s3% chmod 777 test3 test5
c4r6s3% ls -l
total 16
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwx--xr-- 1 ehunda 2025_london 4 Jun  1 21:46 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-rwxrwxrwx 1 ehunda 2025_london 2 Jun  1 23:44 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-rwxrwxrwx 1 ehunda 2025_london 1 Jun  1 23:44 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Jun  1 22:20 test6 -> ex02/
c4r6s3% ln test3 test5
c4r6s3% ls -l
total 16
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwx--xr-- 1 ehunda 2025_london 4 Jun  1 21:46 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-rwxrwxrwx 2 ehunda 2025_london 2 Jun  1 23:44 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-rwxrwxrwx 2 ehunda 2025_london 2 Jun  1 23:44 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Jun  1 22:20 test6 -> ex02/
c4r6s3% ln -l
ln: invalid option -- 'l'
Try 'ln --help' for more information.
c4r6s3% ls -l
total 8
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwx--xr-- 1 ehunda 2025_london 4 Jun  1 21:46 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-rwxrwxrwx 2 ehunda 2025_london 0 Sep  3 16:10 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-rwxrwxrwx 2 ehunda 2025_london 0 Sep  3 16:10 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Jun  1 22:20 test6 -> ex02/
c4r6s3% cat > test3
a%                                                                                                      c4r6s3% ls -l
total 16
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwx--xr-- 1 ehunda 2025_london 4 Jun  1 21:46 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-rwxrwxrwx 2 ehunda 2025_london 1 Sep  3 16:10 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-rwxrwxrwx 2 ehunda 2025_london 1 Sep  3 16:10 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Jun  1 22:20 test6 -> ex02/
c4r6s3% touch -d "2025/06/01 23:44" test3
c4r6s3% chmod -R 504 test3
c4r6s3% ls -l
total 16
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwx--xr-- 1 ehunda 2025_london 4 Jun  1 21:46 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-r-x---r-- 2 ehunda 2025_london 1 Jun  1 23:44 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-r-x---r-- 2 ehunda 2025_london 1 Jun  1 23:44 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Jun  1 22:20 test6 -> ex02/
c4r6s3% chmod -R 404 test3
c4r6s3% ls -l
total 16
drwx--xr-x 2 ehunda 2025_london 6 Jun  1 20:47 test0
-rwx--xr-- 1 ehunda 2025_london 4 Jun  1 21:46 test1
dr-x---r-- 2 ehunda 2025_london 6 Jun  1 22:45 test2
-r-----r-- 2 ehunda 2025_london 1 Jun  1 23:44 test3
-rw-r----x 1 ehunda 2025_london 2 Jun  1 23:43 test4
-r-----r-- 2 ehunda 2025_london 1 Jun  1 23:44 test5
lrwxrwxrwx 1 ehunda 2025_london 5 Jun  1 22:20 test6 -> ex02/
c4r6s3% 
c4r6s3% 
