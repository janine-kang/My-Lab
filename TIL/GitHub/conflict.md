# Conflict Situation



1. 혼자 작업할 때

| final(directory) |   experiment(directory)    |
| :--------------: | :------------------------: |
|  edit `file.md`  | edit `file.md` differently |
|      `push`      |                            |
|                  |           `push`           |
|                  |        !! failed !!        |
|                  |           `pull`           |
|                  |            edit            |
|                  |           `push`           |

- 일치하지 않는 곳부터 `>>>>HEAD`로 표시됨





2. 협업할 때

|      |      |
| ---- | ---- |
|      |      |
|      |      |
|      |      |

