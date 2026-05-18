# Do: Booklab Renewal Prototype

- Feature ID: `booklab-renewal`
- Date: 2026-05-18
- Phase: PDCA Do
- Scope: `module-1,module-2`
- Design: `docs/02-design/features/booklab-renewal.design.md`

## Decision Record Chain

| Source | Decision | Rationale |
|---|---|---|
| PRD | 북랩을 상담 전환형 출판 플랫폼으로 재배치 | 좋은땅의 상담 전환 구조를 벤치마킹하되 북랩의 가격/POD/POS 강점을 전면화하기 위해서 |
| Plan | MVP는 홈, 상담 CTA, 목적 기반 패키지 추천, 출판 과정, 신뢰 섹션 중심 | 제안서와 1차 리뉴얼 설득에 필요한 범위를 명확히 제한하기 위해서 |
| Design | 정적 리뉴얼 프로토타입을 우선 제작 | 기존 CMS 제약 없이 제안서에 바로 캡처 가능한 결과물을 만들기 위해서 |

## Context Anchor

| Anchor | 내용 |
|---|---|
| WHY | 정보 나열형 출판사 사이트를 상담 전환형 출판 플랫폼으로 바꿔 상담 문의와 출간 신청 전환을 높인다. |
| WHO | 첫 책을 준비하는 개인 저자, 전문가/강사 저자, 소량 제작이 필요한 단체/학교/가족 프로젝트 고객. |
| RISK | 기존 레거시 사이트/CMS 구조, 가격 정보 관리, 좋은땅과의 유사성, 상담 폼 항목 과다, 후기 콘텐츠 부족. |
| SUCCESS | 상담 신청 전환율 +30%, 출간 신청/원고 전송 클릭률 +20%, 패키지 상세 진입률 +25%, 모바일 CTA 클릭률 +30%. |
| SCOPE | module-1은 제안서용 홈 구조와 카피, module-2는 반응형 스타일과 모바일 CTA 구현이다. |

## Implementation Summary

| Module | Output | Status |
|---|---|---|
| module-1 | `prototype/booklab-renewal/index.html` | Revised after feedback |
| module-2 | `prototype/booklab-renewal/styles.css` | Revised after feedback |

## Revision Note

사용자 피드백에 따라 기존의 추상적인 카드/목업 중심 시안을 폐기하고, 루트 `DESIGN.md`의 쿠팡형 디자인 시스템을 반영해 다시 작성했다. 주요 변경 사항은 다음과 같다.

- `DESIGN.md` 기준 반영: `#D42931` 레드 CTA, 검색바, 촘촘한 그리드, 0-4px 샤프한 카드, 높은 정보 밀도.
- 좋은땅 벤치마킹 명확화: 상담 CTA 반복, 책 소개, 화제의 책, 랭킹, 저자 인터뷰, 출판 가이드, FAQ 구조를 화면에 직접 노출.
- 이미지 밀도 강화: 외부 이미지 기반 `<img>` 요소 30개를 사용해 도서/저자/출판 과정/랭킹형 콘텐츠가 많은 랜딩으로 재구성.
- 북랩 차별화 유지: 가격 투명성, POD 제작, POS 판매 확인을 별도 신뢰 섹션으로 유지.

### 2026-05-18 Current Booklab Content Revision

추가 피드백에 따라 다시 수정했다. 이번 버전은 사용자가 제공한 현재 북랩 메인 HTML의 실제 콘텐츠를 기준으로 한다.

- 메인 비주얼 배너: `출간문의`, `인세 받는 즐거움`, `책 판매부수 공개`
- 출판 서비스 3대 배너: `출판유통`, `출판도구 모음`, `인쇄 및 제본`
- 명예의 전당: 세종도서/진중문고 선정 도서와 실제 표지
- 북스토어: 추천 도서와 신간 도서 표지
- 작가 셀프 인터뷰: 황일성, 최성표, 서태수 인터뷰 콘텐츠
- 북랩 NEWS / 북랩 Story / 상담전화 / 결제 안내
- 하단 빠른 메뉴: 원고전송, 원고정서 가이드, 나의 출판계약서, 내 책 홍보하기, 출판가이드북, 무료 본문 템플릿, 도서유통망, 도서판매량 및 인세
- 우측 퀵 메뉴: 원고전송, 결제, 무이자 할부, 저자구매, 배송조회, 도서목록 다운로드 등

## Files Created

## 2026-05-18 Renewal Correction

사용자 피드백에 따라 현재 북랩 홈페이지를 1:1로 복제하는 방향을 중단하고, 기존 북랩 메인의 실제 콘텐츠를 재료로 사용하되 좋은땅 메인에서 확인되는 상담 전환형 흐름으로 다시 재구성했다.

- 좋은땅 참고점: 상단의 출판 상담 진입, 저자 대상 메시지, FAQ/고객센터 노출, 도서 이야기와 저자 인터뷰가 이어지는 콘텐츠 허브 구조
- DESIGN.md 반영점: `#D42931` 중심 CTA와 검색바, 촘촘한 카드 그리드, 0-4px 반경, 이미지 중심 정보 밀도
- 북랩 고유 콘텐츠 반영점: 출간문의 배너, 출판유통/출판도구/인쇄제본, 명예의 전당, 북스토어 신간, 작가 셀프 인터뷰, NEWS/Story, 원고전송/계약서/홍보/판매량 메뉴
- 수정 방향: 기존 테이블형 홈페이지를 그대로 옮기지 않고, 리뉴얼 제안서에 넣을 수 있는 현대적인 메인 흐름으로 재배치

Updated files:

- `prototype/booklab-renewal/index.html`
- `prototype/booklab-renewal/styles.css`

### 2026-05-18 Visual Refinement Pass

사용자 요청 7개 항목을 반영해 이미지 의존형 배너와 빠른 메뉴를 HTML/CSS 기반 리뉴얼 UI로 정리했다.

- 메인 배너: 기존 통이미지 배너 대신 책 표지, 상담 CTA, 핵심 수치를 조합한 신규 히어로 비주얼로 교체
- Service 섹션: 하위 메뉴를 이미지맵/이미지 버튼이 아니라 실제 HTML 버튼으로 전환
- 신뢰 콘텐츠: 이미지가 잘리지 않도록 동일 비율 프레임과 `object-fit: contain` 중심으로 수정
- 명예의 전당/북스토어: 장식 헤더, 설명문, 강조 피처 카드, 도서 카드 hover 상태 추가
- 작가 셀프 인터뷰/NEWS/Story: 섹션 설명, 카드 상단 포인트 바, 인터뷰 워터마크 등 디자인 요소 추가
- 결제 영역: 이미지 배너 제거 후 전화번호/신용카드/무통장입금 HTML 카드로 전환
- 빠른 메뉴: 이미지 버튼 제거 후 이니셜 아이콘과 텍스트 설명 카드로 전환

### 2026-05-18 DESIGN.md Re-read Pass

루트 `DESIGN.md`가 Kakao 기반 디자인 시스템으로 변경되어 프로토타입 스타일을 다시 맞췄다.

- 4px 각진 카탈로그 스타일에서 12px 라운드 중심의 부드러운 카드/버튼/입력 스타일로 변경
- 검색바를 빨간 테두리형에서 `#F0F0F0` 채움형 20px 라운드 검색 UI로 변경
- 강한 그라데이션, 무거운 그림자, 과한 3D 효과를 제거하고 평면적인 배경 색상 레이어링으로 정리
- 전체 여백과 섹션 간격을 넓혀 Kakao식 “대화형/친근한/숨 쉬는” 레이아웃으로 조정
- 텍스트 색상 체계를 `#222222`, `#333333`, `#666666`, `#999999` 중심으로 정리
- 도서/인터뷰/결제/빠른메뉴 카드를 `#ffffff`, `#F8F8F8`, `#E5E5E5` 기반의 플랫 카드로 변경

### 2026-05-18 KRDS Re-read Pass

루트 `DESIGN.md`가 KRDS 기반 디자인 시스템으로 다시 변경되어 프로토타입 CSS를 공공서비스형 명료성/접근성 기준으로 재정렬했다.

- Pretendard GOV 우선 폰트, 본문 17px, line-height 1.5 적용
- 1200px 컨테이너, 24px gutter, 8-point grid 기반 간격으로 조정
- Primary 액션 `#d42931`, pressed/link `#0B50D0`, subtle panel `#ECF2FE` 토큰 반영
- 검색 입력을 KRDS 입력폼에 가깝게 56px 높이, `#58616A` 보더, 8px radius로 변경
- 모든 인터랙션 요소에 4px focus ring 토큰을 추가
- 카드/패널은 흰색 배경, 명확한 1px 보더, 8~12px radius 중심으로 조정
- Primary 색상은 장식 배경이 아니라 CTA, 활성 링크, 포커스 등 행위 중심으로 제한

| File | Purpose |
|---|---|
| `prototype/booklab-renewal/index.html` | 좋은땅 벤치마킹 기반 북랩 리뉴얼 홈 구조와 제안 카피 |
| `prototype/booklab-renewal/styles.css` | 데스크톱/모바일 반응형 레이아웃, CTA, 신뢰 섹션, 패키지 카드 스타일 |

## Success Criteria Coverage

| Criteria | Coverage |
|---|---|
| SC-01 첫 화면 핵심 가치/신뢰 수치/상담 CTA/패키지 추천 CTA | Hero section implemented |
| SC-03 대표 패키지 4개 이상 목적 중심 비교 | Package card section implemented |
| SC-04 출판 과정 6단계 표시 | Publishing journey implemented |
| SC-05 모바일 상담 CTA 접근 | Mobile sticky CTA implemented |
| SC-06 가격 투명성/POD/POS 홈 노출 | Booklab Difference section implemented |
| SC-07 좋은땅 구조 벤치마킹 + 북랩 고유 메시지 유지 | Benchmark diagnosis and differentiation sections implemented |

## Next Scope

Recommended next command:

```text
/pdca do booklab-renewal --scope module-3
```

`module-3`에서는 패키지 추천 질문/결과와 FAQ 토글을 실제 인터랙션으로 구현한다.
## 2026-05-18 Coupang Re-read Pass

Root `DESIGN.md` changed back to a Coupang-based design system, so the renewal prototype was realigned to a dense commerce UI instead of the previous public-service/KRDS tone.

- Removed the KRDS-style 17px body rhythm, public-service input border, and `#ECF2FE` panel tone.
- Restored a compact 14px Pretendard stack with `letter-spacing: -0.02em`.
- Re-tokenized the UI around Coupang Red `#d42931`, pressed `#C73D17`, near black `#111111`, and neutral border `#E5E8EB`.
- Updated the search area to a 48px red-bordered bar with an attached red search button and 4px radius.
- Tightened main, service, trust, bookstore, interview, news, story, payment, and quick-menu sections around 8-12px catalog spacing.
- Kept trust/book cover thumbnails on contained, equal-ratio frames so images do not crop or break.
- Preserved HTML-based service buttons, payment banners, and quick-menu items instead of reverting to image buttons.
