1. Working Directory 설정
	$ mkdir -p Unix/git/test1-git
	$ cd Unix/git/test1-git
	//gitinit명령으로 Working Directory 설정
	$ git init
	//git status명령으로 현재 작업 디렉토리의 상태를 확인
	$ git status
	//Working Directory에 README.md파일 생성
	$ echo 'Test Git Project' > README.md
	$ git status
	//지금 작성하고있는 내용으로 수정한뒤 2단계로 넘어감
	
2. 작업물을 Working Directory에서 Staging Area 이동
	//git add 명령으로 파일을 Untracked에서 Staged상태로 변경
	$ git add README.md
	$ git status

3. 로컬 저장소에 반영
	//git commit 명령으로 파일을 Staged상태에서 Unmodified상태로 변경
	$ git commit
	$ git status
	//git log 명령어로 Git의 히스토리 조회
	$ git log
	
4. 원격 저장소에 반영
	$ git remote add origin https://github.com/../unixtest.git
	$ git branch -M main
	$ git push -u origin main
	github ID, 토큰 입력
