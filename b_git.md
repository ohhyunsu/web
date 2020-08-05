# 깃이란 무엇인가?
 
 소프트웨어 개발 및 관리에서 자료를 버전/기간/작성내용순서에 따라 문서를 관리하는 버전관리시스템 이라고 한다.<br />
 이는 한사람이 혼자 작업을 진행 할 수도 있지만, 하나의 데이트를 여러사람이 관리하여 처리 할 수도 있다.

 ---

 ## 핵심 키워드

- git clone 깃주소
- git config --global user.name "사용자 이름"
- git status
- git add 파일 또는 폴더명
- git commit -m "내용요약"
- git config --global user.email "사용자 이메일"
- git push
- git pull
- git reset HEAD^ 가장처음 취소 컨트롤제트기능

---

## 깃 사용법 기초 1

1. 컴퓨터에 연결할 사용자의 계정을 등록한다.(사용자 이름, 이메일주소)
```shell
$ git config --global user.name "ohhyunsu"
$ git config --global user.email "hiohhyunsu@gmail.com"
```

2. github사이트에서 개인 저장소를 생성한다.
- 사이트에서 `new repository`를 클릭
- 이름생성, 자료공개여부(공개), readme파일생성여부

3. 내컴퓨터에서 github사이트에 있는 주소에 담긴 자료를 그대로 복제한다.
- 웹에 존재하는 github저장소이름이 내컴퓨터에 폴더명으로 저장되기 때문에 이름이 겹치지 않도록 주의
``` shell
$ git clone http://---------------.git
```

4. 최초의 테스트 및 파일인식은 `README.md`파일 생성 후 내용 작성

```shell
$ touch README.md
$ echo "readm파일 생성 및 체크" >> README.md
```

5. 선택자료를 첨부 및 내용요약작성 그리고 전송
``` shell
$ git add 파일/폴터 선택
git add . 점이나 * 찍으면 전부다 첨부
$ git commit -m "첨부되는 내용을 요약작성"
$ git push 
```

6. 자료를 상태정검은 수시로 해야한다.

```shell
$ git status
```

7. 혹여 다른 컴에도 clone 되어 있는 상태라면, 서버의 자료를 업데이트로 설정해야 한다.
```shell
$ git pull
```
