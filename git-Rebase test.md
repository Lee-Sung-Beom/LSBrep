# Rebase Test

이전의 Repository에서 Rebase 진행이 온전하지 않아 새로운 Repo 생성 후 Rebase 진행

지금까지 진행한 과정을 반복한 후 Rebase 까지 test

    - Lee-Sung-Beom/Rebase-test: Rebase를 위한 origin/master(원본 저장소)
    - LSB-sub/Rebase-sub: Rebase를 위한 Sub Repo(sub 저장소)

- 로컬 저장소에 Lee-Sung-Beom/Rebase-test 연결

    1. SourceTree에서 Add를 통해 Rebase-test 추가
        > Rebase-test 폴더 생성 후 "Git Base"를 통해 다음의 명령어 진행
        ```sh
        $ git init
        $ git config --global user.name "Github name"
        $ git config --global user.email "Github email"
        ```
    2. Rebase-test 연결 후 VScode를 사용하여 파일 생성 후 커밋 진행
        > File 이름 = Rebase test 1  
        > Commit = First commit in Rebase-test Repo
        ```sh
        $ git commit -m "First commit in Rebase-test Repo"
        ```
    3. 커밋 완료 후 Push 진행
        > SourceTree에서 Push를 통해 원격 저장소인 Rebase-test로 올리기
        

