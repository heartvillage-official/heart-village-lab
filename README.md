# 하트빌리지 세포변화연구소 — GitHub Pages 공개용 V1.1

운영 표기: **자담인 부산사랑점 · 하트빌리지**  
현재 자료: 2026년 11월 9일 7DAY 1일차. 2~6일차 강의는 아직 등록하지 않았습니다.

## 1. 폴더 구조

```text
index.html
.nojekyll
assets/
  research-lab-entrance.jpg
  research-lab-interior.jpg
  research-cell-profile.jpg
data/
  lectures.json
  new-lecture-template.json
README.md
```

**ZIP 파일을 압축해제한 후 최상위 `index.html`, `assets`, `data` 폴더 등을 그대로 저장소 최상위에 업로드하세요.** ZIP 자체만 업로드하면 사이트가 실행되지 않습니다.

## 2. GitHub Pages 만들기

1. GitHub에서 새 저장소 생성 (예: `heart-village-lab`). 개인 무료 요금제의 Pages라면 공개 저장소가 필요합니다.
2. 이 압축파일의 **안쪽 파일과 폴더를 모두** 저장소 루트에 업로드 (`Add file` → `Upload files` → `Commit changes`).
3. 저장소 `Settings` → `Pages` → `Build and deployment` → `Deploy from a branch` → `main` / `(root)` → `Save`.
4. 배포 후 표시되는 `Visit site` 주소 접속. 보통 `https://사용자명.github.io/heart-village-lab/` 같은 주소입니다.
5. 공개 사이트에는 실명, 의료·건강 정보, 강의 전문 등을 게시하기 전에 필요한 허락과 정확성을 검토하세요. GitHub Pages 공개 사이트의 내용은 누구나 볼 수 있습니다.

## 3. 매일·매달 강의 기록 업데이트

- **파일은 `data/lectures.json` 한 곳을 수정합니다.** 첫 기록 `HV-2026-11-D01` 뒤에 쉼표로 구분하여 새 객체를 추가합니다. `new-lecture-template.json`의 구조를 참고합니다.
- `date`는 실제 강의일(`YYYY-MM-DD`), `day`는 월별 1~6일차 숫자, `title`과 `summary`는 원문에 맞는 내용, `tags`는 검색용 주제, `sections`는 자세한 연구노트의 본문입니다.
- JSON 파일은 유효한 형식이어야 합니다. 예를 들어 배열 항목 사이 쉼표 누락이나 마지막 항목 뒤의 불필요한 쉼표에 주의하세요.
- GitHub 웹사이트에서 파일을 편집한 뒤 `Commit changes`를 하면 게시된 웹사이트가 갱신됩니다. 주민이 별도 파일을 다시 받거나 재설치할 필요가 없습니다.
- 새 달의 기록을 등록하면 월 선택 목록에도 자동으로 나타납니다. 7일짜리 프로그램 지도는 그대로이며 강의 아카이브에 월별로 누적됩니다.
- 지금 DAY 01의 10개 화면은 `index.html`에 내장된 학습 여정입니다. 새 달의 복잡한 10개 화면도 추가하려면 페이지 템플릿화가 다음 개발 과제입니다. 현재 새 기록은 `sections`로 상세 본문을 읽을 수 있습니다.
- **주의:** 공개 페이지에 로그인·관리자 권한이 없으므로 주민이 사이트에서 입력해 게시하는 기능은 제공하지 않습니다. 모두에게 보이는 자료는 GitHub 저장소에서 변경해야 합니다.

## 4. 사진이 안 나올 때

- `assets` 폴더가 `index.html`과 같은 상위 폴더에 있는지, 대소문자와 파일명이 정확한지 확인하세요.
- HTML은 `assets/research-lab-entrance.jpg` 같은 **상대 경로**를 사용합니다. GitHub Pages의 저장소 주소 하위에서도 작동합니다.
- 이 패키지의 이미지는 JPEG로 크기를 줄여 포함했습니다. 원본 이미지가 없어도 화면에 이미지가 뜹니다.

## 5. 앞으로 더 편리하게 운영하고 싶다면

1단계: GitHub Pages + JSON 직접 업데이트 (지금 제공).
2단계: 승인된 운영자만 로그인해 글을 입력·검수·발행할 수 있는 관리자 화면과 CMS/데이터베이스 도입. Supabase/Firebase 같은 데이터베이스 또는 Git 기반 CMS 사용을 검토하세요. 이 기능은 현재 패키지에 포함되지 않았습니다.
3단계: 월별 연동 자동화, 검색 개선, 강의 공개 승인 워크플로, 콘텐츠 백업, 도메인 연결.

## 6. 출처·공개 범위

사이트는 제공된 강의의 편집 자료입니다. 원문을 임의 수정하지 않고, 자동 전사 오류가 있는 원본은 공개 전에 교정·검수하세요. 강의자·본사의 배포 허용 범위를 확인한 자료만 게시하세요. 질병 치료·섭취량 등에 관한 발언을 의학적으로 검증된 일반 지침으로 표현하지 마세요.
