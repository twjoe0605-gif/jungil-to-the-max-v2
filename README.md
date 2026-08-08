# 중일투더맥스 · 조태욱

중일고등학교 영어교사 조태욱(중일투더맥스)의 프로필 사이트.
도전 · 성장 · 나눔을 축으로 영어교육과 AI·디지털 교육 활동을 기록합니다.

**배포:** Vercel · **구조:** 의존성 없는 정적 사이트 (빌드 단계 없음)

## 구성

```
index.html          전체 페이지 (HTML/CSS/JS 인라인, 외부 의존성 없음)
assets/
  hero.mp4                        히어로 영상 (1920×1080, 5초)
  teacher-portrait.webp           인물 이미지
  jump-higher-brand.webp          JUMP HIGHER 브랜드 포스터
  material-confirmation-bias.jpg  수업 자료 — 확증편향
  material-smart-goods.jpg        수업 자료 — 스마트 테크 굿즈
  material-question-map.jpg       수업 자료 — 환경 질문 수업
```

## 페이지 구성

히어로 → 브랜드 캐러셀 → 01 WHO I AM → 02 가치 → 03 학교 → 04 전문성 →
05 경력 → 06 활동 → 07 AI 연수 → 수업자료 캐러셀 → 채널 → 문의

## 디자인 메모

- **밴드 교차** — 홀수 섹션은 크림/잉크, 짝수 섹션은 남색 `#16265E` 고정.
  각 밴드가 `--fg` `--gold` `--coral` 등 자기 토큰을 재정의하므로,
  라이트·다크 어느 테마에서도 밴드별 대비가 스스로 맞는다.
- **테마** — `prefers-color-scheme` + `data-theme` 양방향 오버라이드.
- **캐러셀** — `.reel` 요소마다 독립 인스턴스로 초기화된다.
  `.reel--fit` 은 4컷 만화처럼 잘리면 안 되는 자료용(`object-fit:contain`).
- **한글 조판** — `word-break: keep-all` 로 어절 단위 줄바꿈.
- **영상 소리** — 브라우저가 소리 있는 자동재생을 막으므로,
  무음 자동재생 + 사용자가 누르는 소리 토글 방식.

## 로컬에서 보기

빌드가 필요 없습니다. `index.html` 을 브라우저로 열거나:

```bash
python -m http.server 8000
```

## 링크

- YouTube — https://youtube.com/@ddingle
- 강의 문의 — Google Form (사이트 하단 버튼)
