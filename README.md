# 오픈소스 스튜디오 01분반

22300650 / 전도원

### Assignment 1-1. My First Web Page

한동대학교 오픈소스스튜디오 과제 01.
AI를 활용해 자기소개 웹페이지를 제작하고, Git/GitHub로 버전을 관리한 뒤 Vercel로 배포하는 과정을 실습한 프로젝트입니다.
index.html은 AI로 생성한 원본이고, index2.html은 이를 복사해 직접 수정한 페이지입니다.

## Deploy

Vercel Deploy: https://2026-oss-a01.vercel.app/
index.html: https://2026-oss-a01.vercel.app/index.html
index2.html: https://2026-oss-a01.vercel.app/index2.html

# Weekly Review

## Key Learning

1. Git 명령어
   git clone, add, commit, push, pull, branch, status, remote -v, remote add 등 기본적인 git 명령어들을 복습하고, 배웠습니다.

2. Vercel을 통한 배포 방법
   Vercel을 저장소에 한 번 연결해 두면, 이후에는 push만으로 빌드와 배포가 자동 실행된다는 것을 배웠습니다.

3. DevTools의 수정은 화면에만 적용되는 일시적인 변경이다.
   Elements 탭에서 CSS 값을 바꾸면 화면은 즉시 바뀌지만 새로고침하면 원래대로 돌아오며, 실제 반영은 반드시 소스 파일을 수정해야 한다는 것을 확인했습니다.

## Development Flow

VS Code → HTML 작성/수정 → Git commit → GitHub push → Vercel 자동 배포 → Web

로컬에서 작성 및 수정한 내용을 커밋하여 버전관리를 하고, 푸시를 하여 원격 저장소에 저장했습니다. 원격 저장소를 Vercel에 연결하여 자동 배포를 실시하였고, 연결 이후에는 수정사항을 저장하고 push하면 별도 작업을 거치지 않고 Vercel 측에서 이를 자동으로 감지 후 배포하는 것을 실제 배포된 URL에 접속하여 확인했습니다.

## Code Modification

index.html -> index2.html에서 수정한 주요 내용입니다.

- 이미지 추가: 원본에는 이미지가 없었으나, About 섹션에 프로필 사진(`images/profile.png`)을 추가.
- 배치 변경: About 섹션 소개 글과 사진을 나란히 배치.
- 외부 링크 추가: Links 섹션에 한동대 전산전자공학부(HGU CSEE) 링크 추가.
- 스타일 변경: 메인 타이틀 크기를 clamp(56px, 12.5vw, 172px)에서 200px까지 키우고, 본문 폰트 크기를 clamp(16px, 1.35vw, 18px)로 통일.
- 텍스트 변경: 자기소개 문구를 "웹, 앱, 그 너머"에서 "AI, Web, App 그 너머"로 수정하는 등 소개 내용을 재작성함.
- 불필요한 코드 삭제: 사용하지 않게 된 .standfirst 관련 CSS와 코드 제거.

## Problem & Solution

문제
About 섹션에 소개 글과 프로필 사진을 나란히 배치하고 싶었지만, 어떻게 구현해야 할지 몰라 방법을 찾아봐야 했습니다.

해결
flex를 이용하면 소개 글과 사진을 가로로 나란히 배치할 수 있다는 것을 찾아 적용했습니다. 그런데 데스크톱에서는 의도대로 보였지만 브라우저 창을 줄이면 텍스트가 담기는 폭이 급격히 좁아져 한 줄에 몇 글자밖에 들어가지 않는 문제가 새로 생겼고, 이를 해결하는 과정에서 반응형 처리까지 함께 배우게 되었습니다. DevTools의 반응형 모드로 화면 폭을 줄여가며 레이아웃이 깨지는 지점을 확인하는 법을 알았고, about-box의 flex-direction을 column으로 바꿔 좁은 화면에서는 사진이 글 아래로 내려가도록 했습니다.
나란히 배치하는 방법을 찾다가, 화면 폭에 따라 배치 방향 자체를 바꾸는 반응형 처리까지 배우게 되었습니다.

## Reflection

프로필 사진을 넣으면서 img 태그를 어떻게 쓰는지 검색해 봤는데, src만으로 충분하지 않고 alt 속성을 함께 넣는 것이 좋다는 설명을 보게 되었습니다. 스마트 기기의 화면 낭독기가 alt 태그의 텍스트를 읽어 시각장애인 사용자에게 이미지의 내용을 전달한다는 것을 알게 되었습니다.
지금까지는 이런 태그가 있는 줄 전혀 몰랐었는데, 앞으로 이렇게 배려하는 마음을 가지고 개발하고 싶다고 생각했습니다.
