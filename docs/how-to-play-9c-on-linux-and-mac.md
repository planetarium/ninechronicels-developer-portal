---
title: Play 9c on x86 macOS / Linux using CI Artifacts (UNOFFICIAL SUPPORT)
---
# 1. Get Artifact

## [1. 9c-launcher CircleCI 파이프라인 페이지에 들어간다](https://app.circleci.com/pipelines/github/planetarium/9c-launcher?branch=main)

![Untitled](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Untitled.png)

[여기다.](https://app.circleci.com/pipelines/github/planetarium/9c-launcher?branch=main)

## 2. 초록색 체크된 최상위 build-{자기 OS}를 클릭한다.

![Screenshot_20220729_190921.png](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Screenshot_20220729_190921.png)

## 3. Artifacts를 클릭

![Screenshot_20220729_191617.png](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Screenshot_20220729_191617.png)

![Screenshot_20220729_191604.png](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Screenshot_20220729_191604.png)

## 4. Artifact 다운로드 → 압축 풀기

![Screenshot_20220729_1916172.png](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Screenshot_20220729_1916172.png)

![Screenshot_20220729_1916042.png](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Screenshot_20220729_1916042.png)

클릭해서 tar.gz를 받아준다.

## 5. OS에 맞는 파일 압축 풀기

리눅스 유저는 **Linux.tar.gz**

인텔맥 유저는 **macOS.tar.gz**

**압축을 풀어준뒤, 압축 풀린 디렉터리에서 `curl [https://download.nine-chronicles.com/9c-launcher-config.json](https://download.nine-chronicles.com/9c-launcher-config.json) -o resources/app/config.json` 을 터미널로 반드시 실행해준다!**

# 2. Run on Linux

![Untitled](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Untitled%201.png)

압축을 풀면 대충 이렇게 생겨먹었다.

아마 보통은 Nine Chronicles를 클릭하면 실행이 되기는 할텐데

나는 터미널에서 `./Nine Chronicles`를 입력해서 실행하는것을 선호한다. 특별한 이유는 없다.

![Untitled](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Untitled%202.png)

잘 된다.

설정 파일은 보통 `~/.config/Nine Chronicles`에 있다. Libplanet.Tools 또는 [`planet`](https://github.com/planetarium/libplanet/releases) 이라고 부르는 그 CLI 프로그램을 이용해서 개인 키를 임포트 해올 수 있다. 또는 알아서 패스 찾아서 윈도우 마운트 한다음에 거기서 키스토어 폴더에 개인키 UTC뭐시기 파일을 찾아서 여기 설정 폴더에 넣어줘도 된다. 그건 설명하지 않아도 잘 할 수 있으리라고 여러분을 신뢰해본다.

## 2.1. TroubleShooting

### 2.1.1. Ubuntu 22.04의 .NET core 3.1 설치에 관해 (220729 @Hyeon)

1. [https://docs.microsoft.com/en-us/dotnet/core/install/linux-ubuntu#supported-distributions](https://docs.microsoft.com/en-us/dotnet/core/install/linux-ubuntu#supported-distributions) 에 따르면 dirsto 의 OpenSSL v3 제약으로 인해 .NET core 3.1 은 공식적으로 지원하지 않는다.
2. 일단 .NET 6.0 을 깔고 3.1은 tarball 을 받아서 밀어넣는 식으로 해결할 수 있다.
    1. .NET 6.0 은 공식 문서 따라가면 apt로 간단하게 깔 수 있다.
3. [https://dotnet.microsoft.com/en-us/download/dotnet/3.1](https://dotnet.microsoft.com/en-us/download/dotnet/3.1) 에서 자신의 아키텍처에 맞는 binary 를 다운받는다. (모르겠으면 일단 x64를 받고 보자.)
4. 압축을 풀면 여러개의 폴더가 보인다. 이거랑 `/usr/share/dotnet` 의 내용을 비교하며 내용을 합친다.
    1. 폴더를 까보면 `/usr/share/dotnet` 쪽에 6으로 돼있고 압축을 푼 쪽에는 3으로 된 폴더가 나오는 곳이 있다. 6이 있는 자리에 3을 살포시 합석시켜주면 된다.
5. 작업이 끝나고 터미널에서 `dotnet --list-sdks` 를 했을 때 3.1, 6.0 두개가 보이면 성공.

### 2.1.2. 🗯️안돼요!

당황하지 말아라. 침착해야 한다. 충분히 그럴 수 있다. 

가끔씩 검은 창이 떴다 꺼지거나, 커맨드라인에 GPU process isn't usable 이라며 굳바이를 날리는 때가 있다. 그럴때는 커맨드라인을 열고 `./Nine Chronicles` 뒤에 `--no-sandbox` 또는 `--in-process-gpu`를 붙히면 잘된다. 왜 그런지는 모르겠다. 구글이 그랬다.

### 2.1.3. 🗯️런쳐 화면이 하얘요!

작동엔 문제 없더라. 하지만 로그를 #9c-launcher 에 올려주시면 런처팀이 좋아합니다.

### 🗯️게임이 실행 안됐는데 스타트 버튼도 없어요!

#9c-launcher의 사람들을 호출해주면 감사드리겠습디다.

# 3. Run on Intel Mac

![Untitled](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Untitled%203.png)

~~일단 맥을 짚어본다~~

나는 맥이 없다.

그래도 설명할만큼은 친절하다.

압축풀면 이렇게 생겼다.

맥이 있는 사람이 그러길, 압축을 풀고 Nine Chronicles.app을 누르면 실행된다더라.

보안 옵션이 뭐라 하거든, 우클릭해서 오픈해주면 열건지 물어볼건데 연다고 하면 실행된다더라.

→ 그냥 실행하면 안되는데 쓰레기통 버릴래? 라고 물어본다 버리지 말고…

 @Yoshi System Preference → Open Anyway 클릭

![Screen Shot 2022-06-30 at 6.49.33 PM.png](9c%E1%84%85%E1%85%B3%E1%86%AF%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%90%E1%85%A6%E1%86%AF%E1%84%86%E1%85%A2%E1%86%A8%20%E1%84%85%E1%85%B5%E1%84%82%E1%85%AE%E1%86%A8%E1%84%89%E1%85%B3%E1%84%8B%E1%85%A6%E1%84%89%E1%85%A5%20%E1%84%91%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%92%E1%85%A2%E1%84%87%E1%85%A9%E1%84%8C%E1%85%A1!%20d6a8e3f576b544db8ab0345f81a7aaa9/Screen_Shot_2022-06-30_at_6.49.33_PM.png)

참으로 신기하지 않을 수 없다.

## 3.1. TroubleShooting

### 3.1.1. 🗯️도와줘요! 뭐가 안돼요!

나는 맥없는 행인이오. 그대를 돕고 싶으나 나의 맥이 한없이 부족함을 탓하시오.

# 4. Run on Mac (Apple Silicon)

<aside>
💡 유경험자의 기록 요청합니다

</aside>

# -끝-