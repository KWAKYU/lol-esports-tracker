# 🏆 LoL Esports 2026 — Season Tracker

**Live site → https://kwakyu.github.io/lol-esports-tracker/**

League of Legends e스포츠 2026 시즌을 한 페이지로 따라가는 트래커입니다.
백엔드 없이 **HTML 파일 하나**로 동작하며, 라이엇의 일정 발표에 맞춰 스스로 갱신됩니다.

An auto-updating League of Legends esports tracker for the 2026 season.
A **single HTML file** — no backend, no build step. Open it and it keeps itself up to date.

---

## ✨ 주요 기능 / Features

**🗺️ 시즌 로드맵 / Season roadmap**
- First Stand → Road to MSI → MSI → Summer → Worlds를 한눈에 보는 타임라인
- 지난 단계 ✓, 현재 단계 `NOW` 표시, 실제 일정 데이터 기반 날짜
- A visual timeline of the whole season — finished stages get a ✓, the current stage a pulsing `NOW`

**📅 경기 & 브래킷 / Matches & brackets**
- 전 지역(LCK · LPL · LEC · LCS · LCP · CBLOL) + 국제대회 경기 일정과 결과
- 대진표(브래킷) 자동 렌더링 — MSI 진출 시드 박스, 정규시즌 순위표 포함
- 라이브 경기는 YouTube / Twitch / SOOP 시청 링크와 함께 표시
- Interactive bracket view with MSI seed boxes and regular-season standings; live matches link to streams

**❓ 입문자 친화 설명 / Beginner-friendly explainers**
- 각 단계마다 "누가 / 방식 / 걸린 것"을 풀어주는 설명 패널
- 시드, Bo5, 더블 엘리미네이션, 스위스 스테이지 등 용어 사전 내장
- 경기 카드를 누르면 **실제 대진표 데이터에서 계산한** 승/패 시 행선지를 보여줌
- Click any match to see exactly what's at stake — computed from the real bracket graph, not guesswork

**🌐 한/영 전환 / KO–EN toggle**
- 우측 상단 🌐 버튼으로 전체 UI 전환, 선택은 자동 저장

**🔄 자동 갱신 / Auto-refresh**
- 45초마다 데이터 갱신 — 경기가 시작되면 자동으로 LIVE 표시

---

## 🚀 사용법 / Usage

그냥 접속하면 됩니다: **https://kwakyu.github.io/lol-esports-tracker/**

로컬에서 쓰려면 `index.html`을 내려받아 브라우저로 열면 끝입니다. 설치·빌드 과정이 없습니다.

To run locally, download `index.html` and open it in any browser. No install, no build.

---

## 🔧 동작 방식 / How it works

- 데이터: 비공식 LoL Esports 피드(`esports-api.lolesports.com`)를 브라우저에서 직접 호출
- 일정 → 시즌 단계 자동 분류, 대진표는 `getStandingsV3`의 매치 그래프로 레이아웃 자동 계산
- 시간은 접속자의 로컬 시간대로 표시
- All data is fetched client-side from the unofficial LoL Esports feed; the bracket layout is computed
  automatically from the match dependency graph

## ⚠️ 참고 / Disclaimer

Riot Games와 무관한 **비공식 팬 프로젝트**입니다. 비공식 API를 사용하므로 라이엇 측 변경 시 동작이 멈출 수 있습니다.

Unofficial fan project, not affiliated with or endorsed by Riot Games. Uses an unofficial API that may change without notice.
