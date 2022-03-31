# [KDT] 핀테크 서비스 백엔드 개발자 양성 과정 - 워크시트 이민형 1주차

- ## 2022-03-28
    - ### Linux
        - 리누즈 토발즈가 작성한 커널 혹은 GNU 프로젝트의 라이브러리와 도구가 포함된 운영체제
        
        - Kernal
            - 하드웨어와 응용프로그램을 이어주는 운영체제의 핵심 시스템소프트웨어
        - Shell
            - 운영체제의 커널고 ㅏ사용자를 이어주는 소프트웨어

        - 명령어
            |명령어|의미|
            |---|---|
            |cd|경로이동|
            |cat|텍스트파일 내용보기|
            |vi|Vim 에디터로 열기|
            |mkdir|디렉토리 생성|
            |pwd|현재 경로확인|
            |touch|텍스트형식 파일 생성|
            |mv|파일이동|
            |rm|파일삭제|
            |rm -rf|디렉토리 삭제|


    - ### Markdown

    ~~~
    <!-- 주석표기 -->
        
    <!-- 제목 텍스트 -->
    # h1
    ## h2
    ### h3
    #### h4
    ##### h5
    ###### h6
    
    <!-- 순서없는 리스트(- * + 혼용 가능) -->
    - Item1
        - Item1-1
            - Item1-1-1
    * Item2
    + Item3
        

    <!-- 순서있는 리스트 -->
    1. Item1
    2. Item2
        
    <!-- 하이퍼링크 -->
    '''
        [링크 텍스트](링크 URL)
    '''
        
    <!-- 이미지 -->
    '''
        ![대체 텍스트](이미지 URL)
    '''
        
    <!-- 강조 표기 -->
    '''
        *Italic*
        **Bold**
        ~Line Break~
        _Single underscore_
    '''
    
    <!-- 인용문(Blockquote) -->
    '''
        > 인용할 문장
    '''
    
    <!-- Code 입력(문장 내) -->
    This is how `code` works.
    
    <!-- Code 입력(블록) -->
    ' ''' '
        def say_hello():
            return "hello"
    ' ''' '

    <!-- 수평선 -->
    '''
        Page 2

        ***
        Page 2

        -----
        Page 3
    '''
    ~~~
---
<br>

- ## 2022-03-29, 2022-03-30
    - ### Git Bash
        - 명령어
            |명령어|의미|
            |---|---|
            |git config --global user.name "**username**"|git의 username 설정|
            |git config --global user.email "**email**"|git의 email 설정|
            |git config --list|git의 설정값 출력|
            |git init|새로운 local Repository 생성|
            |git status|현재 git의 상태 확인|
            |git clone **저장소URL**|현재 디렉토리에 해당 git clone|
            |git add|staging Area로 작업한 파일 add|
            |git commit|local Repository로 변경사항 commit|
            |git push|remote Repository로 commit한 파일 push|
            |git push origin **브랜치명**|commit한 내용을 remote repository에 push|
            |git branch|local branch 리스트 출력|
            |git branch -m master main|branch명을 master에서 main으로 변경|
            |git branch **브랜치명**|local branch 생성|
            |git branch -D **브랜치명**|local branch 삭제|
            |git switch **브랜치명**|local branch 이동|

        - ### Commit Convention
            |Commit frefix|용도|
            |---|---|
            |feat: *내용*|**새로운 기능**을 추가할 경우|
            |docs: *내용*|**문서파일**을 생성하거나 수정한 경우|
            |conf: *내용*|**설정파일**을 생성하거나 수정한 경우|
            |test: *내용*|**테스트**를 추가, 리펙토링 했을경우|
            |fix: *내용*|**올바르지 않은 동작**을 고친 경우|
            |refactor: *내용*|동작을 더 **괜찮게** 고쳤을 경우|
            |ci: *내용*|**CI 관련 설정**을 수정한 경우|
            |build: *내용*|**빌드 관련 파일**을 수정한경우|
            |perf: *내용*|**성능을 향상**시키는 코드로 변경한경우|
    
    - ### Git flow
        -
            |명령어|의미|
            |---|---|
            |git flow init|git-flow의 사용 시작|
            |git flow release start RELEASE **이름**|develop 브랜치로부터 release 브랜치 생성|
            |git flow release publish RELEASE **이름**|release commit 허용을 위해 게시|
            |git flow release finish RELEASE|release브랜치를 main 브랜치에 병합(merge)  <br> release브랜치를 release이름으로 태그 후  <br>release브랜치를 develop 브랜치로 재병합(back-merge)  <br>release브랜치 삭제
            |git push --tags|tag 들을 push|
            |git flow feature start **이름**|브랜치를 생성하고 그 브랜치로 전환|
            |git flow feature finish **이름**|현재 브랜치를 develop에 merge(병합)후 현재 브랜치 삭제|
            |git flow feature publish **이름**|원격 서버에 게시 (git push)|
            |git flow feature pull origin **이름**|다른 사용자가 게시한 기능 가져오기(git pull)|
        
