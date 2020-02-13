# Window 가상환경 만들기

- 파이썬 설치

  - [https://www.python.org/downloads/](https://www.python.org/downloads/)

  - 설치 파일 실행

    - page 1
      - Customize installation
      - add Python 3.7 to PATH
    - page 2
      - 모두 체크(Documentation, pip, test suite...)
    - page 3(Advanced Options)
      -  Install for all users
      - Associate files with pyhton
      - Create shortcut
      - Add python to env variables
      - precompile standard library
    - 끝

  - 도스 명령어/Windows PowerShell(관리자) 실행

    - 윈도우 > 우클리 > 관리자(A)

  - 파이썬 설치된 패키지 확인

    - ```python
      > pip list
      ```

  - ```python
    cd \w	#설치 위치로 이동
    PS C:\w> python -m venv p3	#virtual enviroment <폴더이름>
    ```

  - Virtual env 사용

    - ```python
      PS C:\w> cd \
      PS C:\w> p3\scripts\activate.bat
      ```

    - 매번 windows powershell을 새로 열었을 때 batch 파일을 실행시켜 주어야 한다.

- SciPy.org 파이썬 패키지군 설치

  - ```python
    PS C:\w> python -m pip install numpy scipy matplotlib ipython jupyter pandas sympy nose
    ```

  - ```python
    PS C:\w> pip list	#엄청 많이 설치되어있음
    ```

- cmd 열기

  - ```python
    C:\User\MinGI.Kim> cd\
    C: cd p3\scripts activate.bat		#BATCH 파일 실행
    ```

- 환경변수 등록(디렉토리 이동 수 activate.bat 을 매번 하지 않기 위해)

  - Path 정보에 가상환경 정보가 설정된 후에 명령프롬프트 실행후 바로 `activate`만 입력하면 가상환경이 활성화 된다
  - 내 PC > 속성 > 고급 시스템 설정 > 고급 > 환경 변수(N) > 사용자 변수의 PATH > 편집
  - `C:\p3\Scripts` 새로 만들기

- cmd 열기

  - ```python
    C:\User\MinGi.Kim> activate
    ```

- 쥬피터 실행

  - ```python
    (p3) C:\> jupyter notebook
    ```

- 라이브러리 패키지 설치 방법

  - activate
  - pip install scikit-learn
  - pip install tensorflow