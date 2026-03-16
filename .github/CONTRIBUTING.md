# GitHub Collaboration Guide

이 문서는 프로젝트 협업을 위한 기본 규칙을 설명합니다.

---

# 1. Branch 전략

브랜치 구조

main  
→ 배포 가능한 안정 버전

develop  
→ 개발 통합 브랜치

feature/*  
→ 기능 개발

bugfix/*  
→ 버그 수정

refactor/*  
→ 코드 개선

예시

feature/csi-preprocessing  
bugfix/mqtt-timeout

---

# 2. 작업 흐름

1. Issue 생성
2. Branch 생성
3. 기능 개발
4. Pull Request 생성
5. 코드 리뷰
6. develop 브랜치에 merge

---

# 3. Branch 생성 규칙

브랜치 이름 형식

type#이슈번호

예시

feature#1  
bugfix#2

---

# 4. Commit Message 규칙

형식

type: 내용

예시

feat: CSI 데이터 전처리 기능 추가  
fix: MQTT 연결 오류 수정  
docs: README 업데이트

사용 가능한 type

feat  
fix  
docs  
refactor  
test  
chore

---

# 5. Pull Request 규칙

PR 생성 전 확인

1. develop 브랜치 기준으로 생성
2. 코드 빌드 확인
3. 테스트 완료

PR 제목 형식

[type] 내용

예시

[Feature] Implement CSI preprocessing

---

# 6. Code Review 규칙

PR은 최소 1명 이상의 리뷰를 받아야 merge 가능

리뷰 항목

- 코드 가독성
- 기능 정상 동작
- 중복 코드 여부
- 예외 처리

---

# 7. Issue 작성 규칙

Issue에는 다음 내용을 포함

- 문제 또는 기능 설명
- 구현 방향
- 완료 기준

---

# 8. Label 규칙

feature → 기능 개발  
bug → 버그  
task → 일반 작업  
documentation → 문서

---

# 9. Merge 전략

merge 방식

Squash merge 사용

이유

- commit history 정리
- 변경 내용 추적 용이