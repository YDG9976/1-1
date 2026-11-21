# 1-1

```bash
# 경로 확인
$ pwd
/c/Users/ehdrb99769976/Desktop/1차시
# 파일 만들기
$ touch A

# 폴더 파일 속 파일들 확인
$ ls
A

# 모든 파일의 경로까지 확인
$ ls -a
./  ../  A

# 파일들의 권한을 확인
$ ls -l
total 1
-rw-r--r-- 1 ehdrb99769976 1049089 13 Nov 21 12:41 A

# 모든 하위 파일의 경로, 권한 확인
$ ls -la
total 0
drwxr-xr-x 1 ehdrb99769976 1049089 0 Nov 21 12:39 ./
drwxr-xr-x 1 ehdrb99769976 1049089 0 Nov 21 12:38 ../
-rw-r--r-- 1 ehdrb99769976 1049089 0 Nov 21 12:39 A

# 경로 이동
ehdrb99769976@GNIA-C202-D03 UCRT64 ~/Desktop/1차시
$ cd
ehdrb99769976@GNIA-C202-D03 UCRT64 ~

# 폴더가 아닌 파일로 이동 시도
$ cd A
bash: cd: A: Not a directory

# 존재하지 않는 경로로 이동 시도
$ cd B
bash: cd: B: No such file or directory

# 파일 만들기
$ touch B

# 폴더 만들기
$ mkdir File

# 카피
$ cp A File

# 이동
$ mv B FIle
'''b 파일이 사라지고 c 폴더 안에 b가 생긴것을 확인'''

# 삭제
$ rm A
'''a 파일이 사라짐'''

# 폴더 삭제
$ rm -r File
'''c 폴더가 사라짐'''

# 내용 쓰기
$ echo "hello world!" > A
'''메모장으로 실행하면 hello world!가 적혀있음'''

# 내용 읽기
$ cat A
hello world!

# 권한 변경
root@91482fa81423:/File# touch A
root@91482fa81423:/File# ls -l
total 0
-rw-r--r-- 1 root root 0 Nov 21 03:54 A
root@91482fa81423:/File# chmod 777 A
root@91482fa81423:/File# ls -l
total 0
-rwxrwxrwx 1 root root 0 Nov 21 03:54 A
```
