# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 프로젝트 개요

이 레포지토리는 Jekyll 기반의 GitHub Pages 이력서 프로젝트입니다. `sproogen/resume-theme`를 사용하여 개인 이력서 웹사이트를 생성합니다.

## 빌드 및 실행 명령어

### 로컬 개발 서버 실행
```bash
bundle exec jekyll serve
```

### 의존성 설치
```bash
bundle install
```

### 빌드
```bash
bundle exec jekyll build
```

## 프로젝트 구조

- `_config.yml`: Jekyll 사이트의 주요 설정 파일. 개인정보, 경력, 프로젝트 등 모든 이력서 내용이 YAML 형식으로 정의됨
- `index.md`: 홈페이지 추가 콘텐츠 (경력 하이라이트)
- `_site/`: Jekyll이 생성한 정적 사이트 파일들 (자동 생성됨)
- `images/`: 프로필 이미지 등 이미지 파일들
- `assets/`: SCSS 스타일시트

## 주요 설정 및 수정 방법

### 콘텐츠 수정
모든 이력서 내용은 `_config.yml` 파일에서 관리됩니다:
- 개인정보: `name`, `title`, `email`, `phone` 등
- 경력사항: `content` 섹션의 첫 번째 항목
- 프로젝트: `content` 섹션의 두 번째 항목
- 교육/활동: 나머지 `content` 섹션들

### 테마 설정
- Ruby 버전: 2.7.2
- Jekyll 테마: `sproogen/resume-theme` (remote theme)
- 다크모드: 비활성화 (`darkmode: never`)

## 배포

이 프로젝트는 GitHub Pages를 통해 자동으로 배포됩니다. `main` 브랜치에 push하면 자동으로 사이트가 업데이트됩니다.

## 개발자 프로필 특성

### 강조하는 가치
- **성능 최적화**: 모든 개선사항을 구체적인 수치로 표현 (예: 15초→5초, 800ms→400ms)
- **실용적 접근**: 오버엔지니어링을 피하고 적절한 기술 선택
- **체계적 문제 해결**: 원인 분석 → 해결방안 → 결과 측정의 논리적 흐름
- **팀워크**: 기술적 우수성과 함께 팀 문화 기여 중시

### 이력서 작성 시 주의사항
- 성능 개선은 반드시 Before/After 수치로 표현
- 디자인 패턴 적용 시 구체적인 패턴명과 효과 명시 (전략 패턴, 추상 팩토리 패턴 등)
- 문제 해결 과정을 스토리텔링으로 구성
- 비즈니스 가치와 기술적 성취의 균형 유지
- 레거시 코드 개선 경험 강조

### 주간업무 작성 패턴
- **구조**: 작업 배경 → 주요 구현 포인트 → 처리 방식/고려사항
- 기술적 디테일과 비즈니스 맥락 함께 기록
- 발생한 문제는 "문제상황 → 원인 분석 → 해결방안" 형식으로 정리
- 코드 예시나 SQL 쿼리는 백틱으로 표시
- 처리 건수나 성능 수치 등 정량적 데이터 포함

### 기술 문서 작성 스타일
- 트레이드오프를 명확히 제시 (예: Local Cache vs Global Cache)
- 실제 구현 코드와 함께 설명
- 선택한 기술의 이유를 실용적 관점에서 설명
- 도표나 이미지를 활용한 시각적 설명 선호