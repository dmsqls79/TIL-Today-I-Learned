## 20180726_Python_day4

* Python 
0 - false
1 - true
Ex) not 3%3 —> not 0(false) —> True 이용해서 조건 적용 가능
“fizz” * True —> ‘fizz'
“fizz” * False —> ‘'
‘ ‘ or 1 —> 1


* FILE I/O
- open().write().close()
f = open(‘file name’, ‘mode’)   //   ./—>경로지정
f.close() —> 한 세트
-mode(w-쓰기(매 순간 파일 업데이트/누적 아님) / r-읽기 / a(append)-추가)

Write mode
f.write(내용)

Read mode
f.readline(맨 윗줄 하나만 읽음-커서 기준으로 한 줄씩 읽음)
f.readlines(모든 줄을 읽어냄)—>list로 출력함

- comma spread values
with open(‘file name’, ‘mode’) as f:  —> f=open() f.close()


* Error handle *
try:
    실행문
except error a 이름:
    실행문

* Git 

—Shell— 
.  현재폴더
.. 상위폴더
cd /  경로 이동(change directory)
mkdir	디렉토리 생성
touch 	파일 생성
ls // ls -al 포함된 파일 보여줌
mv file directory/ 파일을 디렉토리로 이동
cp file directory/ 파일을 디렉토리로 복사
mv 이름 이름/ rename
rm 파일 —> 제거
rm -rf directory —> directory 제거
exit —> shell 끝냄

Git 내에서 git 연결하면 안됨
:wq —> 저장하면서 나감
:q! —> 저장안하고 나감

git —version —>깃 버전 보여줌
Python3 —version —> 파이썬 버전 보여줌
python3 파일이름 —> 파일 실행

git init 
git add . —> 깃에 파일 올림
git commit -m “some commit(Vim —> commit message(첫줄 제목/다음 내용))” —> git hub에 새로운 repo 생성

git status —> 상태 보여줌
git remote add origin(어떤 이름이든 가능) 주소
git remote get-url origin —>url 보여줌
git remote show origin —> fetch, push url 보여줌
git add 파일
(Status 확인 : 빨—>초 올라감)
git commit
git push origin master

rm -rf .git —> 현재 상태에서의 깃 떨어져 나감
