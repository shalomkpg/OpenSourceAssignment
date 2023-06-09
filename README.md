# 프로젝트 개요

이 프로젝트는 리눅스 명령어에 대한 설명과 사용 예시를 제공하는 README 문서입니다. 리눅스 운영체제에서 자주 사용되는 명령어들을 다루고 있으며, 각 명령어에 대한 설명과 사용법을 알려줍니다.

## 목표

- 리눅스 사용자들에게 다양한 명령어의 기능과 사용법을 소개하고 설명합니다.
- 명령어를 사용하여 리눅스 시스템을 효율적으로 관리하고 문제를 해결하는 데 도움을 제공합니다.
- 예시 코드와 함께 명령어의 사용법을 실제로 이해하고 익힐 수 있도록 돕습니다.

## 주요 기능

- 다양한 리눅스 명령어에 대한 개요와 설명을 제공합니다.
- 각 명령어의 사용법과 옵션에 대한 예시 코드를 제공합니다.
- 명령어 관련된 외부 링크를 포함하여 보다 상세한 정보를 제공합니다.
- 이미지를 통해 명령어나 예시의 시각적 이해를 돕습니다.

# 리눅스 명령어

## 명령어 개요

| 명령어 | 설명 |
|--------|------|
| [`top`](https://ko.wikipedia.org/wiki/Top_(%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4)) | 시스템의 현재 상태와 실행 중인 프로세스를 실시간으로 모니터링합니다. |
| [`ps`](https://ko.wikipedia.org/wiki/Ps_(%EC%9C%A0%EB%8B%89%EC%8A%A4)) | 현재 실행 중인 프로세스 목록을 표시합니다. |
| [`job`](https://ko.wikipedia.org/wiki/Jobs_(%EC%9C%A0%EB%8B%89%EC%8A%A4)) | 백그라운드에서 실행되는 작업을 관리합니다. |
| [`kill`](https://ko.wikipedia.org/wiki/Kill_(%EB%AA%85%EB%A0%B9%EC%96%B4)) | 실행 중인 프로세스를 종료시킵니다. |

## `top` 명령어

`top` 명령어는 시스템의 현재 상태와 실행 중인 프로세스를 실시간으로 모니터링하는 유틸리티입니다. 명령어를 실행하면 다음과 같은 정보를 확인할 수 있습니다:

- 시스템 CPU 및 메모리 사용량
- 실행 중인 프로세스 목록
- 프로세스별 CPU, 메모리 사용량 등 세부 정보

### 사용 예시

```bash
$ top
```

![BSD-unix-top-plain](https://github.com/shalomkpg/OpenSourceAssignment/assets/133830026/a74d41d9-e358-414c-9035-30e117753290)

## `ps` 명령어

`ps` 명령어는 현재 실행 중인 프로세스 목록을 표시하는 유틸리티입니다. 다양한 옵션을 사용하여 원하는 형식으로 출력할 수 있습니다. 주요 옵션은 다음과 같습니다:

- `-e`: 시스템 전체 프로세스 표시
- `-f`: 자세한 출력 포맷 사용
- `-u <사용자>`: 특정 사용자의 프로세스만 표시

### 사용 예시

```bash
$ ps
$ ps -e
$ ps -f
$ ps -u <사용자>
```

![PPID](https://github.com/shalomkpg/OpenSourceAssignment/assets/133830026/172e5cfb-b300-4479-bb4e-062f24aeb33b)

## `job` 명령어

`job` 명령어는 백그라운드에서 실행 중인 작업을 관리하는 유틸리티입니다. 다음과 같은 기능을 제공합니다:

- 현재 실행 중인 작업 목록 표시
- 작업을 일시 중지하거나 다시 시작
- 작업을 백그라운드 또는 포그라운드에서 실행

### 사용 예시

```bash
$ job
$ job <작업번호>
```

## `kill` 명령어

`kill` 명령어는 실행 중인 프로세스를 종료시키는 유틸리티입니다. 프로세스를 종료시키기 위해 해당 프로세스의 식별자(PID)를 사용합니다. 명령어를 실행할 때 다양한 옵션을 지정하여 특정한 종료 시그널을 보낼 수 있습니다.

일반적으로 사용하는 옵션은 다음과 같습니다:

- `-9`: 강제로 프로세스를 종료시킵니다.
- `-15`: 프로세스에 종료 시그널을 보내 정상적으로 종료시킵니다.
- `-l`: 사용 가능한 종료 시그널 목록 표시

### 사용 예시

```bash
$ kill <PID>
$ kill -9 <PID>
$ kill -15 <PID>
$ kill -l
```
