# `git push` 실행시 로그인 정보 묻지 않도록 변경하기(SSH 키 설정)

## SSH 키 생성하기

SSH key를 설정하기 위해서는 터미널에서 아래의 명령어를 입력합니다. 명령어 입력 후 세 번의 입력은 엔터키를 입력해서 넘어갑니다.

````sh
$ ssh-keygen -t rsa
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/USERNAME/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /Users/USERNAME/.ssh/id_rsa.
Your public key has been saved in /Users/USERNAME/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx USERNAME@COMPUTER
The key's randomart image is:
+---[RSA 2048]----+
|o..              |
|+ooo             |
|B+++ ..          |
|**oo*..o         |
|B+o.o+. S        |
|=+.=....         |
|.EB..oo .        |
|o+. .+ .         |
|*.oo+..          |
+----[SHA256]-----+
$
````

이렇게 하면 `~/.ssh`에 공개키와 비밀키가 생성됩니다. 확인을 위해 아래의 명령어를 입력해보세요.

````sh
$ ls ~/.ssh

id_rsa id_rsa.pub
````

.pub가 붙은 건 공개키, 안붙은 건 비밀키입니다. 그럼 이제 공개키를 깃허브의 설정에 추가해보겠습니다.

## 생성한 SSH 키를 깃허브에 등록하기

깃허브 프로필 페이지에서 우측 상단의 더보기 버튼에서 설정(Settings)를 클릭합니다.

설정의 항목 중 SSH and GPG keys로 이동합니다.

"New SSH key" 버튼을 클릭하여 "Title"에 식별 가능한 이름을 적어줍니다. 원하는 이름으로 하면 됩니다. 떠오르지 않는다면 "ssh-Key"로 만들어보겠습니다.

키 입력 부분에 .id_rsa.pub의 내용을 붙여 넣습니다.

여기까지 마치면 이제 SSH를 이용해 깃허브 저장소에 접근할 수 있습니다.

Github의 저장소에서 "Clone or download" 버튼을 클릭했을 때 나오는 창에서 "Use SSH"를 복사해서 여러분의 프로젝트 디렉토리의 리모트 저장소 설정을 변경해 줍니다.

````sh
$ git remote set-url origin SSH_URL
````

이제 `git push`를 실행할 때 더이상 로그인 정보를 묻지 않습니다.
