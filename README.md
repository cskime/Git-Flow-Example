# Git-Flow-Example
> [Git-Flow 사용하기](https://cskime.github.io/2019/11/git/gitflow/)

## Overview

- Branch
  - master : 개발 완료
  - develop : 개발중
  - feature : 기능 개발
  - release : master 가기 전 테스트
  - hotfix : master에서 버그를 찾았을 때

## Usage

- `start` : 해당 branch 생성하여 작업 시작

- `finish` : 해당 branch 작업을 끝내고 삭제

- 설치

  ```shell
  $ brew install git-flow-avh
  ```
  
- 초기화 : master, develop 생성

  ```shell
  $ git flow init
  ```

- 기능개발 : feature 생성

  ```shell
  $ git flow feature start {name}
  $ git flow feature finish {name}
  ```

- 배포 전 테스트 : release 생성

  ```shell
  $ git flow release start {name}
  $ git flow release finish {name}
  ```

- master에서 버그 수정 : hotifx 생성

  ```shell
  $ git flow hotfix start {name}
  $ git flow hotfix finish {name}
  ```

  