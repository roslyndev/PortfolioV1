# 포트폴리오 v1 프로젝트 참여 가이드

> 환영합니다! 이 프로젝트는 누구나 기여할 수 있는 오픈소스 프로젝트입니다. 아래의 절차를 따라 참여해주세요.


## 브랜치 전략

이 프로젝트는 다음과 같은 3개의 주요 브랜치를 운영합니다.

 - main : 최종 배포 브랜치
 - staging : 테스트 및 검증 브랜치
 - integration : 개발 브랜치 (모든 작업은 여기서 시작됩니다.)


## 기여하는 방법


1️⃣ 이슈 작성 및 할당

> 새로운 작업을 시작하기 전에 반드시 Issues에서 관련 이슈를 작성하거나, 기존 이슈를 확인하고 본인을 Assign하세요.


2️⃣ 개발 브랜치 생성 및 작성

 - `integration` 브랜치에서 새로운 브랜치를 만들어 작업을 진행하세요.
 
```bash

git checkout integration
git pull origin integration
git checkout -b feature/your-feature-name

```

3️⃣ PR(Pull Request) 생성

 - 작업이 완료되면 `integration` 브랜치로 PR을 생성하세요.
 - PR에는 관련된 이슈 번호를 연결하여, 이슈가 해결될 수 있도록 해주세요.
 
```html
 - resolve #13 -> 이슈번호 연결
```

 - 리뷰어를 지정하고 코드 리뷰 요청을 진행합니다.


4️⃣ 코드 리뷰 및 머지

 - 최소 1명 이상의 리뷰어가 승인해야 머지가 가능합니다.
 - 리뷰 후 문제가 없다면 `integration` 브랜치로 머지가 됩니다.


5️⃣ staging 브랜치로 PR 요청

 - integration에 반영된 코드 중 배포할 기능을 선별하여 staging 브랜치로 PR을 요청합니다.
 - PR이 승인되면 staging에 머지됩니다.


6️⃣ main 브랜치로 자동 PR 및 배포

 - `staging`에서 머지된 변경 사항은 자동으로 main 브랜치로 PR이 생성됩니다.
 - 관리자가 최종 검토 후 승인하면 main에 머지가 되고, GitHub Actions를 통해 서비스가 배포됩니다.
 - 배포된 내용은 지정된 URL에서 확인할 수 있습니다.


## 추가 규칙

 - PR을 생성하기 전에 반드시 관련 이슈를 작성하고, 해당 PR이 해결하는 이슈를 Closes #이슈번호 형식으로 연결하세요.
 - 브랜치 명칭은 feature/작업내용 또는 fix/작업내용 형태로 지정하세요.
 - 코드 리뷰는 팀원 간의 협업을 위한 필수 과정이므로, 적극적으로 참여해주세요.

> 프로젝트에 기여해주셔서 감사합니다! 😊
> 궁금한 사항이 있다면 Issues 또는 Discussions을 통해 문의해주세요. 🚀


## Description

 - 본 프로젝트는 포트폴리오용 첫번째 프로젝트입니다.
 - 본 프로젝트는 공개 프로젝트로 함께 작업할 분들을 초청하여 진행됩니다.


### Spec

 - Vue 3.5 composition api
 - TypeScript


