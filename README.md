# Git 워크숍 - 환경설정

본 문서는 Git 워크숍에 앞서 준비해야할 사항에 대한 안내 문서입니다. 이 문서에서는 아래와 같은 내용을 다룹니다.

- 개인 컴퓨터 권장 사양
- 사전설치프로그램의 목록과 설치 방법
- 개인 컴퓨터상의 프로그램 설치 상태를 확인하는 방법
- 깃허브 가입 방법 안내

## 권장 사양

- 윈도우즈 10 권장(최소 윈도우즈 7 이상(VS Code 최소사양))
- 맥OS Mojave 권장(최소 맥OS Yosemite 이상(VS Code 최소사양))

## 사전 설치 프로그램

Git 워크숍에서는 텍스트에디터와 터미널 에뮬레이터를 활용합니다. 입문 단계의 수강생을 기준으로 워크숍을 준비하므로 아직 텍스트에디터와 터미널에 익숙하지 않은 분들이 참석한다는 전제하에 사전 설치 프로그램을 권해드립니다. 만약 기존에 사용하는 프로그램이 있으시다면 반드시 아래의 프로그램을 설치해야하는 것은 아닙니다.

### 윈도우즈/맥OS 사용자 공통

- [비주얼스튜디오 코드(Visual Studio CODE, 이하 VS 코드)](https://code.visualstudio.com/)

### 윈도우즈 사용자

- [Git for windows 2.9.1](https://gitforwindows.org/)

### 맥OS 사용자

- VS 코드 외에 별도의 프로그램을 설치하지 않습니다. 기본 터미널 에뮬레이터가 아닌, 다른 에뮬레이터를 사용하고 싶다면 [iTerm2](https://iterm2.com/)를 설치해도 무방합니다.

## 설치 방법

### 윈도우즈 사용자

- [VS 코드 다운로드 페이지](https://code.visualstudio.com/Download)에서 운영체제에 맞는 설치 파일을 다운로드 하여 설치합니다.
- [Git for windows 2.9.1](https://gitforwindows.org/)에서 `Git-2.19.1-32-bit.exe
` 또는 `Git-2.19.1-64-bit.exe` 중 운영체제에 맞는 설치파일을 다운로드하여 설치를 진행합니다. 설치시 선택옵션은 모두 기본 상태로 두고 "Next"를 클릭해 설치를 완료합니다.

### 맥OS 사용자

- [VS 코드 다운로드 페이지](https://code.visualstudio.com/Download)에서 운영체제에 맞는 설치 파일을 다운로드하여 설치합니다.
- 터미널 에뮬레이터는 기본적으로 설치되어 있습니다.

## 설치 상태 확인

VS 코드는 프로그램 목록에서 아이콘을 클릭하면 정상적으로 실행이 되는지 확인할 수 있습니다.

### 윈도우즈 사용자

"Git for Windows"를 이상없이 설치했다면 프로그램 목록에 "Git Bash"가 보일 것입니다. 해당 아이콘을 클릭해 터미널을 실행합니다. 입력을 기다리는 깜빡거리는 프롬프트가 화면에 나오면 아래의 명령어를 입력합니다.

> git --version

`git version 2.x.x`처럼 버전이 표시되면 깃을 사용할 수 있는 상태입니다.

### 맥OS 사용자

[응용프로그램]->[유틸리티]->[터미널]을 실행합니다. 입력을 기다리는 깜빡거리는 프롬프트가 화면에 나오면 아래의 명령어를 입력합니다.

> git --version

`git version 2.x.x`처럼 버전이 표시되면 깃을 사용할 수 있는 상태입니다.

## 깃허브 가입하기

워크숍에서는 깃의 원격저장소로 [깃허브](https://github.com/)를 이용합니다. 깃허브 첫 화면의 회원가입 폼에 "Username", "Email"과 "Password"를 입력한 후 폼을 제출하면 가입할 수 있습니다. 가입을 완료한 후에는 입력한 이메일 주소로 발송된 인증 메일을 확인해주세요. 메일 인증까지 마치면 깃허브를 이용할 수 있습니다.

## 사전 준비 작업이 어렵게 느껴진다면

대부분의 참가자가 텍스트에디터, 터미널 등 개발에 필요한 툴을 세팅하는 게 처음일 것이라 생각합니다. 사전 설치 작업에 어려움을 느끼신다면 워크숍 진행 전에 연락을 주세요. 해결할 수 있도록 도와드리겠습니다. 해결이 어렵다면 그 상태에서 워크숍에 참석하셔도 괜찮습니다. 부담없이 참석하셔서 함께 하나씩 해결하면 됩니다:smiley:

## 참고사항

- [`git push` 실행시 로그인 정보 묻지 않도록 변경하기(SSH 키 설정)](./docs/set-ssh-key.md);
