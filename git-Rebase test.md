# Rebase Test

이전의 Repository에서 Rebase 진행이 온전하지 않아 새로운 Repo 생성 후 Rebase 진행

지금까지 진행한 과정을 반복한 후 Rebase 까지 test

    - Lee-Sung-Beom/Rebase-test: Rebase를 위한 origin/master(원본 저장소)
    - LSB-sub/Rebase-sub: Rebase를 위한 Sub Repo(sub 저장소)

- 로컬 저장소에 Lee-Sung-Beom/Rebase-test 연결

    1. 로컬저장소와 Rebase-test 연결
        > Rebase-test 폴더 생성 후 "Git Base"를 통해 다음의 명령어 진행
        ```sh
        $ git init
        $ git config --global user.name "Github name"
        $ git config --global user.email "Github email"
        $ git clone <Rebase-test URL>.git  
        # 해당 명령어 사용 시 폴더 내 Rebase-test 폴더 또 생성
        ```
    2. Rebase-test 연결 후 VScode를 사용하여 파일 생성 후 커밋 진행  
        - **_VScode(Visual Studio Code)는 별도의 설정 과정 없이 설치 가능_**
        > 위 과정 진행 시 폴더 내 생성된 Rebase-test 저장소에서 Git Bash 실행  
        > File 이름 = Rebase test 1  
        > Commit = First commit in Rebase-test Repo
        ```sh
        $ git add --all # 폴더 내 모든 파일을 커밋하기 위한 작업
        $ git commit -m "First commit in Rebase-test Repo"
        ```
    3. 커밋 완료 후 Push 진행
        > Push를 위해 Rebase-test 저장소 위치를 특정  
        > Git Bash에서 Push를 통해 원격 저장소인 Rebase-test로 올리기
        ```sh
        $ git remote add origin <Rebase-test URL>.git
        $ git push origin main  
        # 로컬 저장소의 이름은 Git Bash에서 폴더가 위치한 경로 맨 뒤의 ()에 적힌 이름으로 확인 가능
        ```
    4. Github에 접속하여 올라간 파일 확인  
<br>

- SourceTree에서 로컬 저장소 및 Rebase-test 저장소 추가  

    1. SourceTree 설치  
        ```
        1. Install 단계에서는 "Bitbucket"을 사용하여 소셜 계정으로 로그인 하도록 설정  
        2. "You may need to switch accounts" 문구 확인 시 하단의 "sign up for Bitbucket Cloud"를 클릭하여 GIthub에서 사용중인 계정과 동일하게 입력  
        (SourceTree 사용을 위한 계정으로 동일하게 입력)  
        3. "Bitbucket" 가입 완료 후 "Login to Bitbucket" 창 확인 시 "뒤로"  
        4. Registration 단계에서 "Bitbucket" 선택 후 "Grant access"를 사용하여 등록  
        5. Mercurial 사용은 하지 않으므로 체크 해제 후 진행  
        6. SSH 키는 "아니오"를 선택하여 사용하지 않음
        ```
    2. SoucrTree 로그인
        ```
        1. SourceTree 실행 후 좌측 상단의 "Remote"를 선택하고 프로필을 우클릭하여 "계정 편집" 진행  
        2. 호스팅 서비스 = Github 변경  
        3. "OAuth 토큰 새로고침"을 통해 인증  
        4. Github 목록에서 Rebase-test 선택
        ```
    3. SourceTree에 Rebase-test 추가
        ```
        1. SourceTree 실행 후 "Add"를 통해 추가  
        2. "탐색"으로 Rebase-test의 로컬 저장소 선택  
        ```
<br>

- SourceTree에서의 커밋과 푸시  

    1. Rebase test 2 파일 생성  
    