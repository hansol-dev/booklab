# 북랩 리뉴얼 작업 인계 메모

이 저장소는 북랩 홈페이지 리뉴얼 프로토타입 작업용 저장소입니다. 새 터미널이나 새 에이전트 세션을 열었을 때는 이 파일을 먼저 읽고 현재 상태를 이어가세요.

앞으로 `AGENTS.md`는 반드시 한글로 작성합니다.

## 작업 위치

- 루트 경로: `C:\hansol\booklab`
- 메인 프로토타입 경로: `prototype/booklab-renewal/`
- 주요 파일:
  - `prototype/booklab-renewal/index.html`
  - `prototype/booklab-renewal/styles.css`
  - 루트 `index.html`은 Vercel 루트 접속 시 `./prototype/booklab-renewal/`로 이동시키는 역할입니다.
- 사용자가 확인하는 배포 주소: `https://booklab-coral.vercel.app/`

## 현재 디자인 방향

- 기존 북랩 홈페이지를 그대로 복제하는 작업이 아닙니다.
- 북랩의 실제 콘텐츠는 유지하되, 좋은땅 홈페이지처럼 콘텐츠 진입과 상담 전환이 자연스러운 구조로 리뉴얼하는 시안입니다.
- 현재 포함된 주요 영역:
  - 검색, 출판 계약상담 전화번호, 회원 메뉴, GNB가 있는 헤더
  - 모바일 햄버거 메뉴와 1뎁스/2뎁스 아코디언 메뉴
  - 고정 높이의 메인 히어로 슬라이드 배너
  - 출판유통, 출판도구 모음, 인쇄 및 제본 서비스 섹션
  - 명예의 전당, 북스토어/신간도서, 작가 셀프 인터뷰 섹션
  - 북랩 NEWS, 북랩 Story, 결제 및 상담 카드
  - 저자가 바로 쓰는 빠른 메뉴
  - 북랩 회사 정보 기반 footer

## 최근 작업 상태

최근 푸시된 커밋:

- `f1e3a96 Add agent handoff notes`
- `8ccac8f Fix mobile footer layout`
- `9efa150 Adjust mobile payment card layout`
- `a9589b2 Fix story more link alignment`
- `c60b7d6 Improve mobile navigation and section headers`
- `5c2d5f1 Add mobile hamburger menu`

이미 반영된 최근 수정:

- 모바일 footer가 화면 밖으로 밀리지 않도록 수정했습니다.
- 모바일 footer 링크는 2열 버튼형으로 정리했습니다.
- 모바일 결제 및 상담 영역은 신용카드 결제를 왼쪽, 전화번호 안내를 오른쪽에 배치했습니다.
- 하단 `북랩 Story` 카드의 `더보기` 링크를 우측 정렬했습니다.
- 모바일 메뉴는 햄버거 버튼과 아코디언 서브메뉴 방식으로 동작합니다.
- 모바일 타이틀 영역의 필기체 장식과 버튼 위치를 정리했습니다.

## Git 및 배포

- 원격 저장소: `https://hansol-dev@github.com/hansol-dev/booklab.git`
- 브랜치: `main`
- Git 명령은 보통 `safe.directory` 옵션이 필요합니다.
  - `git -c safe.directory=C:/hansol/booklab status --short`
  - `git -c safe.directory=C:/hansol/booklab add <파일>`
  - `git -c safe.directory=C:/hansol/booklab commit -m "<메시지>"`
  - `git -c safe.directory=C:/hansol/booklab push`
- 푸시는 이전 세션에서 다음 prefix로 승인된 적이 있습니다.
  - `git -c safe.directory=C:/hansol/booklab push`
- GitHub에 푸시하면 Vercel이 자동 배포합니다. 라이브 URL 확인은 푸시 후 약간의 대기 시간이 필요합니다.

## 이 프로젝트의 수정 규칙

- 수동 파일 수정은 `apply_patch`를 사용합니다.
- 검색은 우선 `rg`를 사용합니다.
- 사용자가 만든 다른 변경사항은 되돌리지 않습니다.
- 루트에 `mobile.png`라는 미추적 스크린샷 파일이 있습니다. 사용자가 명시적으로 요청하지 않으면 커밋하지 않습니다.
- PowerShell의 `Get-Content`는 한글이 깨져 보일 수 있습니다. 파일 자체가 깨진 것으로 단정하지 말고 `rg` 또는 브라우저 렌더링 기준으로 확인합니다.
- CSS 수정 후에는 괄호 개수를 확인합니다.
  - `$css = Get-Content -Raw -Path prototype/booklab-renewal/styles.css; $open = ([regex]::Matches($css, '\{')).Count; $close = ([regex]::Matches($css, '\}')).Count; "open=$open close=$close"`
- JS를 수정했다면 커밋 전 문법 확인 또는 세심한 검토가 필요합니다.

## 이미지 및 폰트 자산

현재 사용하는 생성 이미지와 서비스 이미지는 다음 위치에 있습니다.

- `prototype/booklab-renewal/assets/service/main-hero-publishing-journey.png`
- `prototype/booklab-renewal/assets/service/main-hero-distribution.png`
- `prototype/booklab-renewal/assets/service/main-hero-printing.png`
- `prototype/booklab-renewal/assets/service/service-tools-warm.png`
- `prototype/booklab-renewal/assets/service/service-printing-warm.png`

로컬 폰트:

- `prototype/booklab-renewal/assets/fonts/PretendardVariable.woff2`

## 사용자 선호 및 주의점

- 사용자는 한 번에 완성보다 화면을 보면서 하나씩 고치는 방식을 선호합니다.
- 특히 모바일 화면의 간격, 정렬, 버튼 촌스러움, 타이틀 장식 위치를 민감하게 봅니다.
- 기존 북랩 콘텐츠, 메뉴명, 전화번호, 서비스명, 책/뉴스/스토리/인터뷰 콘텐츠는 실제 내용 기반으로 유지해야 합니다.
- 너무 빨간색이 많은 UI를 싫어합니다. 필요하면 붉은색 비중을 줄이고 더 차분한 톤을 제안합니다.
- 한국어 줄바꿈이 어색한 곳에는 `word-break: keep-all`을 적극 사용합니다.
- 화면에 보이는 변경을 완료하면 관련 파일만 커밋하고 `main`에 푸시하는 흐름을 선호합니다.
