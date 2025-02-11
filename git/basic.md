# git 기본 개념

## 분산버전 관리 시스템
클라이언트(우리컴퓨터)와 서버(git hub) 모두가 똑같은 데이터를 유지하여 버전을 관리하는 시스템

## 파일의 세 가지 상태
![areas](../assets/areas.png)

- 영역
    - working directory : 작성하고 있는 코드, 파일
    - staging area : add 명령어로 무대위로 올라간 파일
    - git directory (repository) : commit 명령어로 찍힌 스냅샷들을 저장하는 공간


## 파일의 라이프사이클

![lifesycle]{../assets/lifesycle.png}

워킹 디렉토리의 모든 파일은 크게 Tracked(관리대상임)와 Untracked(관리대상이 아님)로 나눈다. Tracked 파일은 이미 스냅샷에 포함돼 있던 파일이다. Tracked 파일은 또 Unmodified(수정하지 않음)와 Modified(수정함) 그리고 Staged(커밋으로 저장소에 기록할) 상태 중 하나이다. 간단히 말하자면 Git이 알고 있는 파일이라는 것이다.

그리고 나머지 파일은 모두 Untracked 파일이다. Untracked 파일은 워킹 디렉토리에 있는 파일 중 스냅샷에도 Staging Area에도 포함되지 않은 파일이다. 처음 저장소를 Clone 하면 모든 파일은 Tracked이면서 Unmodified 상태이다. 파일을 Checkout 하고 나서 아무것도 수정하지 않았기 때문에 그렇다.