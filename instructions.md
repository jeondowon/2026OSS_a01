과제 목표
개발 환경을 설정 및 AI를 활용하여 간단한 웹페이지를 제작한 후,
Git/GitHub를 이용한 버전 관리와 Vercel 배포 과정을 실습하여 제출합니다.

Development Flow

VS Code → HTML → Git → GitHub → Vercel → Web

수행내용
STEP 1. Development Environment

웹 개발을 위한 기본 환경을 설정합니다.

Visual Studio Code 설치
Front-end 관련 Extension 3개 이상 설치
Git 설치 및 동작 확인
수업용 GitHub Repository 준비
GitHub Repository를 로컬 프로젝트와 연결
Check

VS Code에서 프로젝트 폴더 열기
GitHub Repository에서 프로젝트 확인하기
STEP 2. AI로 My Profile Page 만들기

ChatGPT, Claude 등 AI 도구를 이용하여 자기소개 웹페이지를 제작합니다.

파일명: index.html
AI에게 HTML/CSS 코드 생성을 요청
다음 내용 중 필요한 항목을 자유롭게 구성
이름 또는 닉네임 / 학번 / 전공
관심 분야 / 취미
이번 학기에 배우고 싶은 것
만들어보고 싶은 서비스 또는 프로젝트
HTML Requirements

다음 HTML 요소 중 5개 이상을 사용합니다.

h1~h3, p, div, a, img, ul, li

STEP 3. index2.html 생성 및 코드 수정

AI를 이용하여 생성한 index.html을 복사하여 index2.html 파일을 생성합니다.

index.html : AI를 활용하여 처음 생성한 원본 페이지
index2.html : 원본을 복사한 후 직접 수정한 페이지
index2.html의 소스를 직접 확인하고 다음 중 3가지 이상을 수정합니다.

텍스트 또는 자기소개 내용 변경
글자색 / 배경색 / 글꼴 등 스타일 변경
이미지 추가 또는 변경
외부 사이트 링크 추가
새로운 HTML 요소 추가
페이지의 배치 또는 구성 변경
불필요한 코드 찾아 삭제
수정 후 index.html과 index2.html을 각각 실행하여 변경 전·후의 차이를 확인합니다.

STEP 4. Browser DevTools 사용

index2.html을 브라우저에서 실행하고 Developer Tools를 사용합니다.

Elements에서 HTML 구조 확인
원하는 HTML 요소 선택
CSS 속성 하나 이상 변경
화면의 변화 확인
Console 탭 확인
※ DevTools에서 변경한 내용은 실제 index2.html 파일에 저장되지 않음을 확인합니다.

STEP 5. Git으로 버전 관리

작업 과정을 Git으로 관리하고 최소 2회 이상 Commit합니다.

예) commit message 예시

Create AI profile page

Add customized profile page

Update styles and contents

각 단계에서 GitHub에 Push하고 Commit History를 확인합니다.

STEP 6. Vercel에 배포

GitHub Repository를 Vercel과 연결하여 웹사이트를 배포합니다.

Vercel 회원가입 / 로그인
GitHub Repository Import
Deploy
생성된 URL 접속
index.html 정상 동작 확인
STEP 7. index2.html 추가 → Push → 자동 배포 확인

index2.html을 GitHub에 추가하여 Vercel의 자동 배포 과정을 확인합니다.

index.html을 복사하여 index2.html 생성
index2.html 내용 수정
Git Commit
GitHub Push
Vercel 자동 배포 확인
배포된 index2.html URL 접속 및 정상 동작 확인
예) https://xxxxx.vercel.app/index2.html

핵심 흐름

index2.html 추가/수정 → Commit → Push → GitHub → Vercel Auto Deploy

STEP 8. README.md 작성

GitHub Repository에 README.md 파일을 작성합니다.

다음 내용을 포함합니다.

프로젝트명
프로젝트에 대한 간단한 설명
Vercel Deploy URL
index.html URL
index2.html URL
STEP 9. Weekly Review

README.md에 이번 주 학습 내용을 정리합니다.

Key Learning: 이번 주 배운 핵심 내용 3가지
Development Flow: VS Code → Git → GitHub → Vercel 흐름
Code Modification: index.html에서 index2.html로 변경한 주요 내용
Problem & Solution: 실습 중 발생한 문제와 해결 방법 1가지
Reflection: 새롭게 알게 된 점 또는 궁금한 점 1가지 3. 최종 Repository

index.html — AI를 활용하여 생성한 원본
index2.html — 직접 수정한 페이지
README.md — 프로젝트 및 학습 내용 정리

4. LMS에 제출내역

github repo url
vercel 배포 url 5. Self-Check

AI를 활용하여 index.html 제작
index.html을 복사하여 index2.html 생성
index2.html을 3곳 이상 직접 수정
index.html과 index2.html의 차이 확인
Browser DevTools를 이용하여 HTML/CSS 확인
Git Commit 2회 이상 수행
GitHub Push 및 Commit History 확인
Vercel 배포 완료
index2.html 추가 후 Vercel 자동 배포 확인
index.html, index2.html 모두 URL로 정상 접속
README.md 및 Weekly Review 작성
