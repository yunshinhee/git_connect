# git_connect

#git 설치 방법---> 기본값으로 그대로 설치했음
google에 git검색 
64-bit Git for Windows Setup.다운로드

#시작버튼에서 git bash열기 (실행)

```
GG@DESKTOP-4DR04SQ MINGW64 ~
$ git config --global user.name "whasun"
```

#github 가입 시 입력한 이메일과 동일해야햔다.
```
ESKTOP-4DR04SQ MINGW64 ~
$ git config --global user.email "tlsgml1225@naver.com" 
```


#정보확인하기
```
$ git config --list
```
![image](https://github.com/yunshinhee/git_connect/assets/145514638/f9099e81-3b06-4255-970e-cc198b0bed2c)

🔝위의 내용은 컴퓨터에 한번만 설치하면 됨 

이모키콘 :알파벳 (🥐🥖🍞)
-------------------
-------------------(줄은 짧아도 끝까지 실행됨)



#github에 코드 업로드하기

vs에 업로드할 파일 넣기->VS 창에서 terminal클릭

1.초기화

```
git init
```
#업로드한 파일에 숨김항목 체크 하면 .git이라는 폴더가 생성된다



2.파일 올리기 
```
git add .
```


3.히스토리 만들기
```
git commit -m " 내가 적고 싶은 메세지 "
```
메세지에는 한글이 가능함
-m는 메세지의 준말


4.github repository랑 내 로컬 프로젝트랑 연결(깃업에 프로젝트를 올릴 repository를 먼저 만들어야한다)
예시: webstandard파일 만들기(repository를 만들때 Add a README file체크 X)-commit changes(저장)

#아래 주소는 깃헙에서 만든 repository에서 복사해서 가져와야한다
![image](https://github.com/yunshinhee/git_connect/assets/145514638/3b423407-ac42-4844-9d08-1a0a0b91c1a6)
```
git remote add origin https://github.com/yunshinhee/webstandard.git(복사)
```


5.잘 연결되었는지 확인(필수 아님)
```
git remote -v
```

6.github에 자료 올리기
```
git push origin master
```
![image](https://github.com/yunshinhee/git_connect/assets/145514638/1612da10-9428-49e9-b9e1-34ec61416be5)

창이 뜨면 2번째꺼 누르고 암호 옮겨적기 

#🔝여기까지 하면 github의 repository(webstandard파일)에 자료(원래 파일안에 들어가 있던것 css,img,html 등)가 올라가 있다.
#터미널에서 cls or clear 적으면 초기화 

마지막 netlify에 업로드
Sites -> Add new site ->import an existing project
![image](https://github.com/yunshinhee/git_connect/assets/145514638/711681fe-af4c-4192-8dfc-243f9fd932d0)

![image](https://github.com/yunshinhee/git_connect/assets/145514638/8eb2f0f2-66a5-4d77-bb92-271d131bd510)
원하는 파일 눌러서 클릭 -> Deploy webstandard -> 업로드 되면 파일 이름바꾸기 


