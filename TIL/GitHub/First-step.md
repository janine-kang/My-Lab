### 깃허브 레파지토리 연동하기

> GitHub에 연동하기까지를 작성



|                깃 연결하기                |
| :---------------------------------------: |
|                `git init`                 |
|           create New repository           |
|           create New Directory            |
| `git remote add origin <repository URL\>` |
|                `git add .`                |
|        `git commit -m "*message*"`        |
|         `git push origin master`          |



1. `git init`

```
$ git init
Initialized empty Git repository in C:/Users/YeonokKang/Desktop/last-lab-td/.git/
```


2. `git remote add origin <repository URL\>`

```
$ git remote add origin <repository URL\>
```

* IF ERROR

```
error: remote origin already exists.

$ git remote rm origin

$ git remote add origin <URL\>

```


3. `git add .`  

```
$ git add
```


4. `git commit -m "*message*"`  

```
$ git commit -m "message"
[master (root-commit) b29fa84] message
 1 file changed, 2 insertions(+)
 create mode 100644 Bonnenuit.md
```

*b29fa84 : 파일 코드*

5. `git push origin master`

```
$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 230 bytes | 76.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To <URL\>
 * [new branch]      master -> master
```

##### Done

---



