# vue-project

## 프로젝트 개요
예제 Vue 3 + Vite 앱입니다. TypeScript와 Sass(SCSS)를 사용하며, 구조는 다음과 같습니다.

- `src/main.ts`: 앱 엔트리 포인트
- `src/App.vue`: 루트 컴포넌트
- `src/components/`: UI 구성 요소
- `src/assets/scss/`: 스타일 정의

## 요구 사항
- Node.js 16+ (권장 18, 20)
- npm 9+

## 설치 및 실행
1. 종속성 설치
```bash
npm install
```
2. 개발 서버 실행
```bash
npm run dev
```
3. 브라우저 열기
- 보통 `http://localhost:5173`

## 테스트(없음)
이 프로젝트에는 기본 테스트 스크립트가 설정되어 있지 않습니다. 필요 시 `vitest` 등의 테스트 도구를 추가하시기 바랍니다.

## 빌드 및 배포
```bash
npm run build
npm run preview
```

## 추가 설정(옵션)
### Vue Router
```bash
npm install vue-router@4
```

### Pinia
```bash
npm install pinia
```

## 개발 플로우 요약
- 코드 수정
- `npm run dev` 상태에서 자동 리프레시
- 완료 후 `npm run build`로 최종 패키징


