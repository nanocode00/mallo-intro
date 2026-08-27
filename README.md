# Mallo 소개 정적 페이지

로컬 API, 백엔드, 키오스크 런타임에 의존하지 않는 공개용 정적 소개 페이지입니다.

- `index.html`: 대상별 소개 페이지 선택 진입점
- `customer.html`: 고객·비개발자용 제품/이용 방법 소개
- `evaluator.html`: 평가자·쇼케이스용 구조와 검증 지표 소개
- `styles/intro.css`: 세 페이지가 공유하는 스타일

## 미디어 추가

이미지는 `assets/images/`, 영상은 `assets/videos/`에 넣습니다. 권장 파일명은 각 디렉터리의 README에 정리되어 있습니다. 해당 이름으로 파일을 추가하면 `evaluator.html`이 자동 표시하며, 없을 때는 placeholder가 유지됩니다.

## 정적 호스팅

GitHub Pages에서는 이 디렉터리를 배포 대상(root)으로 지정하거나, Pages가 저장소 루트만 지원하는 경우 빌드/배포 단계에서 `artifacts/intro`의 내용을 사이트 루트로 복사합니다. Vercel에서는 Framework Preset을 `Other`, Root Directory를 `artifacts/intro`으로 지정합니다.
