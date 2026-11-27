# 이게 디자인이야? — 시스테믹 디자인 한눈에 보기

다이어그램으로 시스테믹 디자인을 쉽게 이해할 수 있도록 만든 한 페이지 웹사이트입니다.
JS 프로젝트 스튜디오 2026 기말 프로젝트 초안.

## 구성

| 섹션 | 내용 |
|---|---|
| Hero | "이게 디자인이야?" 질문과 핵심 메시지 |
| 01 Scope | 디자인 대상의 확장 (Buchanan의 네 영역) — 상자를 누르면 설명 표시 |
| 02 Lens | 서비스 디자인 vs 시스테믹 디자인 — 버튼으로 시야 전환 |
| 03 Journey | Systemic Design Toolkit 7단계 + 단계별 대표 도구 — 단계를 누르면 도구 카드 표시 |
| 04 Canvas | 단계별 대표 캔버스 모음과 마무리 메시지 |

## 폴더 구조

```
index.html      페이지 구조와 문구
css/style.css   색상, 글꼴, 레이아웃
js/main.js      데이터(ORDERS, STEPS)와 인터랙션, 도구 섬네일
```

문구를 고치려면 `index.html`, 단계·도구 내용을 고치려면 `js/main.js` 위쪽의 `ORDERS`, `STEPS`를 수정하세요.
색은 `css/style.css` 맨 위 `:root` 변수에서 바꿀 수 있습니다.

## 로컬에서 보기

`index.html`을 브라우저로 열면 됩니다. 별도 빌드가 필요 없습니다.

## GitHub Pages로 올리기

1. GitHub에서 새 저장소를 만듭니다 (예: `systemic-design`).
2. 이 폴더의 파일을 그대로 올립니다 (`index.html`이 저장소 최상위에 있어야 합니다).
   ```bash
   git init
   git add .
   git commit -m "first draft"
   git branch -M main
   git remote add origin https://github.com/<아이디>/systemic-design.git
   git push -u origin main
   ```
3. 저장소의 Settings → Pages → Build and deployment에서 Source를 `Deploy from a branch`, Branch를 `main` / `/ (root)`로 저장합니다.
4. 잠시 후 `https://<아이디>.github.io/systemic-design/`에서 확인할 수 있습니다.

## 출처

- Buchanan, R. (1992). Wicked Problems in Design Thinking. *Design Issues*, 8(2), 5–21.
- Jones, P. (2014). Design Research Methods in Systemic Design. RSD3.
- Jones, P. & Van Ael, K. (2022). *Design Journeys through Complex Systems*. BIS Publishers.
- Systemic Design Toolkit (Namahn · shiftN): https://www.systemicdesigntoolkit.org
- Van Ael et al. (2019). Toolkit hands-on session, RSD8.
- Suoheimo, M., Jones, P., Lee, S.-H. & Sevaldson, B. (Eds.) (2025). *Systemic Service Design*. Routledge.

글꼴: [Pretendard](https://github.com/orioncactus/pretendard) (SIL Open Font License)
