# 오늘의 에러



오늘 주피터 노트북을 이용하여 pymysql과 sqlalchemy를 연동시켰다

pip을 통해 두 패키지를 설치해야하는 줄 알고 무턱대고 했다가 여러 낭패를 봤다.

우선 프롬프터에서부터 막혔는데, 경위는 이러하다.

1. MariaDB를 저번주에 실행시킬 때, root와 python 로그인 비밀번호가 다른줄 몰라서 나머지공부를 했다. 결국 python1으로 아이디와 비밀번호 모두 바꾸어 등록을 마쳤다. 

2. 그런데 오늘 다시 접속을 시도했더니, 안되는 것이다.

   ``` 
   C:\Program Files\MariaDB 10.3\bin> mysql -u python -p
   ERROR 1045 (28000): Access denied for user 'python'@'localhost' (using password: YES)
   ```

   여기에다가 주구장창 비밀번호인 python 1을 넣었다. 에러는 틀린 비밀번호라는 뜻이란다. 틀릴리가 없는데를 반복하다가, 결국 저번주에 python1으로 재설정하던게 기억났다.

3. 애석하게도 python1을 넣을 생각은 못하고 python2로 다시 등록했다. 그러니 또 무한 반복을 하고 있었을 수 밖에. 

4. 마침내 `python2 -p`로 아이디를 변경해서 드디어 로그인을 완료했다.

5. 그러나 진짜 문제는 여기서부터 시작된다. 

   ```
   pip install pymysql
   pip show sqlalchemy
   ```

   를 했을 때, 둘 다 이미 값이 나온 상태였다. 그 말인 즉슨, `sqlalchemy` 패키지가 이미 깔려있다는 소리인데 그것도 모르고 다시 install sqlalchemy를 실행한다. 이게 오류의 시발점인지는 아직도 모르겠다.

6. 결국 짱구를 굴리게 되는데, 가장 단순하게 

7. 

아직도 왜였는지 모르겠다. 











![image-20210111165819204](journal_jan11.assets/image-20210111165819204.png)






