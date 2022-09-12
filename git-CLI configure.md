# CLI 환경의 Git 설치

1. CLI 환경의 Git을 연결하기 위해서는 Git을 설치
2. Git의 로컬저장소로 사용할 폴더에서 Git Bash 실행
3. Git Bash에서의 기본적인 명령어
```sh
$ cd # 홈 폴더로 이동
$ cd Documents/ # 내 문서 폴더로 이동
$ cd <폴더명> # <폴더명> 폴더로 이동
$ cd .. # 현재 폴더의 상위 폴더로 이동
$ pwd # 현재 폴더의 위치 확인
$ ls -a # 현재 폴더의 파일 목록 확인 -a 옵션으로 숨김 파일도 확인
$ mkdir <폴더명> # <폴더명> 폴더 생성
$ git status # Git 저장소의 상태를 알려줌
```
4. 원하는 폴더에서 Git Bash 실행 후 git init 명령어를 통해 Git 로컬 저장소 생성
```sh
$ git init # Git 로컬 저장소 생성
$ ls -a # 파일 목록 확인
$ git status # 현재 상태 확인
```
5. $ git status 명령어를 사용해 현재 Git 로컬 저장소의 상태를 확인 후 옵션 설정
    - 용어 정리
        - 워킹트리: 일반적인 작업이 일어나는 곳
        - 로컬 저장소: .git 폴더, 커밋이 존재하는 곳
        - 작업 폴더: = 워킹트리 + 로컬 저장소
        - Git 저장소: 로컬 저장소를 의미하지만 넓은 의미로 작업 폴더 의미  
  
6. 옵션 설정에는 다음과 같은 config 명령어 사용
```sh
$ git config --global <옵션명> # 지정한 전역 옵션의 내용 확인
$ git config --global <옵션명> <새로운 값> # 지정한 전역 옵션 값을 새로 설정
$ git config --global --unset <옵션명> # 지정한 전역 옵션 삭제
$ git config --local <옵션명> # 지정한 지역 옵션의 내용 확인
$ git config --local <옵션명> <새로운 값> # 지정한 지역 옵션 값을 새로 설정
$ git config --local --unset <옵션명> # 지정한 지역 옵션 삭제
$ git config --system <옵션명> # 지정한 시스템 옵션 확인
$ git config --system <옵션명> <값> # 지정한 시스템 옵션 새로 설정
$ git config --system --unset <옵션명> <값> # 지정한 시스템 옵션의 값 삭제
$ git config --list # 현재 설정된 모든 옵션 확인
```

7. Git 로컬 저장소에서 사용할 user.name과 user.email 입력