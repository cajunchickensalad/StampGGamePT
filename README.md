# STAMP Game — Vercel Static Prototype
- Game Link : 'https://stampgameupdate202609081644.vercel.app/'
- `index.html`: 브라우저에서 직접 실행되는 정적 플레이 테스트 버전
- `data/gameData.json`: `game.db`에서 추출한 게임 데이터
- 별도 서버/API/DB가 필요하지 않습니다.
- Vercel에서는 프로젝트 루트에 `index.html`과 `data/gameData.json`이 있도록 업로드하면 됩니다.

## 이번 수정
- `startPhase()` 누락으로 초기화가 중단되던 문제 수정
- `gameData.json`의 실제 DB 필드명에 맞게 Buffer Type/확률 파싱 수정
- Score Table의 실제 DB 구조(`tier1`~`tier5`)에 맞게 점수 계산 수정
- 상대 경로 `./data/gameData.json` 사용
- 데이터 로드 실패 시 화면에 오류 표시
- WAIT / NEW GAME 버튼 동작 수정
- AI 자동 진행 및 Human 턴 진행 유지
