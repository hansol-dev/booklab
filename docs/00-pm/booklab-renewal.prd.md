# PRD: Booklab Site Renewal

- Feature ID: `booklab-renewal`
- Date: 2026-05-18
- Phase: PDCA PM
- Target site: https://www.book.co.kr/
- Benchmark site: https://www.g-world.co.kr/
- Working title: 북랩 사이트 리뉴얼 - 상담 전환형 출판 플랫폼

## 1. Executive Summary

| 관점 | 요약 |
|---|---|
| Problem | 북랩은 출판 패키지, POD 제작 역량, 판매 조회 등 강점이 있지만 메인 경험이 정보 나열형에 가깝고 첫 방문 저자가 "지금 상담해야겠다"는 확신을 얻기 어렵다. |
| Solution | 좋은땅의 상담 CTA, 신뢰 증거, 출판 과정 가이드, 후기/콘텐츠 구조를 벤치마킹해 북랩을 "비용과 제작 역량이 투명한 출판 파트너"로 재배치한다. |
| UX Effect | 첫 화면에서 핵심 가치, 상담 진입, 추천 패키지, 제작/유통/정산 신뢰 증거를 빠르게 확인하게 하며, 탐색형 메뉴를 저자 여정 중심으로 재구성한다. |
| Core Value | 북랩의 기존 강점인 패키지 가격, POD 생산, 출간 종수, POS 판매 확인을 현대적인 전환 퍼널로 연결해 상담 문의와 출간 신청 전환을 높인다. |

## 2. Product Context

### 2.1 Current Booklab Signals

확인된 북랩 핵심 자산:

- 메인 메시지: "누구나 쉽게 이용할 수 있는 출판 플랫폼"
- 출판패키지: 흑백/컬러/교재/청소년/전자책/50부 프로젝트 등 목적별 상품
- 패키지 가이드: 판형, 색도, 분량, 증정본 기준으로 적합 패키지 안내
- 비용 투명성: 예시 가격표 및 패키지별 기준 사양 제공
- 제작 역량: POD 장비, 자체 제작, 적정 재고 유지, POS 판매 현황 확인
- 회사 신뢰: 2004년 설립, 출간종수 8천 종 돌파, 세종도서 선정 이력

### 2.2 Benchmark: G-World / 좋은땅

좋은땅에서 벤치마킹할 핵심 패턴:

- 상단/메인 CTA가 "출판 상담하기"로 명확하다.
- 출판 과정이 컨설팅, 계약, 교정, 디자인, 인쇄, 유통/마케팅까지 단계형으로 정리되어 있다.
- 저자 후기와 실제 책/저자 콘텐츠가 반복적으로 신뢰를 만든다.
- 도서 제작 현황, 온라인 책장, 인세 계산 등 저자 대시보드 가치를 전면에 노출한다.
- 유통망, 매월 정산, 높은 인세율, 마케팅 프로그램을 불안 해소 메시지로 쓴다.

## 3. Opportunity Solution Tree

### Desired Outcome

예비 저자가 북랩을 방문한 뒤 3분 안에 다음을 판단할 수 있어야 한다.

1. 내 원고에 맞는 출판 방식이 무엇인지
2. 대략 얼마가 들고 어떤 서비스가 포함되는지
3. 북랩이 실제로 믿고 맡길 만한 제작/유통 역량을 갖췄는지
4. 상담 또는 출간 신청을 어디서 시작해야 하는지

### Opportunities

| 기회 | 현재 문제 | 벤치마크 인사이트 | 리뉴얼 방향 |
|---|---|---|---|
| 첫 화면 전환 | 서비스 범위는 넓지만 첫 CTA와 가치 제안이 약하게 보일 수 있음 | 좋은땅은 상담 CTA와 신뢰 메시지를 반복 노출 | 히어로에 "내 책 출판 상담 시작"과 "패키지 추천 받기" 이원 CTA 배치 |
| 패키지 선택 | 상품 종류가 많아 초보 저자에게 복잡할 수 있음 | 좋은땅은 출판 고민을 먼저 다루고 상담으로 유도 | 4문항 진단형 패키지 추천 UX 도입 |
| 신뢰 증거 | 장비/연혁/선정 이력이 하위 페이지에 분산 | 좋은땅은 후기, 수치, 시스템 장점을 본문에 반복 배치 | 출간종수, 세종도서, POD센터, POS 조회를 홈 신뢰 블록으로 승격 |
| 과정 안내 | 단계 정보는 있으나 상담 전환과 결합이 약함 | 좋은땅은 출판 과정 페이지 말미마다 상담 CTA 연결 | "원고 접수부터 서점 유통까지" 6단계 시각화와 단계별 FAQ 제공 |
| 사후 관리 | 판매 및 인세 조회 기능의 가치를 충분히 설명하지 못함 | 좋은땅은 앱/대시보드 기능을 전면 USP로 사용 | MY북랩/POS 판매 조회를 저자 운영 대시보드 가치로 재포지셔닝 |

## 4. Personas

### Persona A: 첫 책을 내는 40-60대 에세이/자서전 저자

- Job to be done: 내 원고를 책으로 만들고 가족, 지인, 독자에게 전달하고 싶다.
- Pain: 출판 과정, 비용, 사기성 업체에 대한 불안.
- Needed proof: 실제 비용, 제작 단계, 담당자 안내, 후기, 전화 상담.
- Product promise: "처음이어도 내 책 사양에 맞춰 출판 방식을 바로 안내받는다."

### Persona B: 강사/전문가/컨설턴트

- Job to be done: 전문성을 증명할 책을 만들고 강연/브랜딩/판매에 활용하고 싶다.
- Pain: 완성도, 디자인 품질, 온라인 서점 유통, 마케팅.
- Needed proof: 제작 품질, 서점 유통, 보도자료/홍보 옵션, 저자 구매가.
- Product promise: "책 제작부터 유통/홍보까지 사업 목적에 맞게 설계한다."

### Persona C: 소량 제작/비매품이 필요한 단체, 학교, 가족 프로젝트 고객

- Job to be done: 50부-300부 수준의 책을 합리적으로 제작하고 싶다.
- Pain: 과도한 최소 부수, 복잡한 옵션, 디자인 파일 준비 부담.
- Needed proof: 50부 프로젝트, 템플릿, 단가표, 납기 안내.
- Product promise: "필요한 부수만, 필요한 옵션만 골라 빠르게 제작한다."

## 5. Value Proposition

### JTBD 6-Part

| 항목 | 내용 |
|---|---|
| Situation | 원고는 있지만 출판 방식, 비용, 유통, 정산이 복잡하게 느껴진다. |
| Motivation | 신뢰할 수 있는 출판사를 통해 책을 만들고 유통하거나 필요한 부수만 제작하고 싶다. |
| Expected Outcome | 내 원고에 맞는 상품과 비용을 이해하고 상담/출간 신청으로 진행한다. |
| Obstacle | 과도한 정보량, 오래된 UI, 후기/신뢰 증거의 낮은 가시성, 패키지 비교 피로. |
| Choice Criteria | 비용 투명성, 제작 품질, 유통 범위, 상담 응답, 사후 판매/정산 확인. |
| Product Role | 저자의 출판 목적을 진단하고 최적 상품, 예상 비용, 다음 행동을 안내하는 출판 플랫폼. |

### Positioning

북랩은 "가격과 제작 역량이 투명한 POD 기반 출판 파트너"로 포지셔닝한다. 좋은땅의 감성적 신뢰/상담 전환 구조를 참고하되, 북랩만의 차별점은 패키지 투명성, 자체 제작/POD, POS 기반 판매 확인, 다양한 목적별 상품으로 둔다.

## 6. Competitive Landscape

| 경쟁/대안 | 강점 | 약점/공략점 | 북랩 리뉴얼 시사점 |
|---|---|---|---|
| 좋은땅 | 상담 CTA, 후기, 과정 안내, 정산/앱 가치 노출이 강함 | 비용/상품 비교가 북랩보다 덜 정량적으로 보일 수 있음 | 신뢰형 UX와 CTA 구조를 벤치마킹하되 가격 투명성으로 차별화 |
| 부크크 | POD/자가출판 인식이 강하고 낮은 진입 장벽 | 초보 저자에게 편집/디자인/마케팅 지원은 제한적으로 느껴질 수 있음 | "전문가가 함께 만드는 출판"을 강조 |
| 교보 POD/퍼플 | 대형 서점 브랜드 신뢰와 POD 유통 접점 | 개인이 직접 처리해야 하는 영역이 큼 | "상담과 제작 대행이 포함된 출판"을 강조 |
| 유페이퍼 | 전자책 셀프출판과 온라인 유통 접근성 | 종이책 제작/디자인/오프라인 유통 니즈에는 약함 | 전자책만이 아닌 종이책+유통+정산의 통합 가치 강조 |
| 일반 자비출판사/인쇄소 | 가격 협상과 오프라인 상담 가능 | 비용/유통/정산 투명성 차이가 큼 | POS 확인, 표준 패키지, FAQ로 불안 제거 |

## 7. Product Requirements

### 7.1 Homepage Requirements

| ID | Requirement | Priority |
|---|---|---|
| H-01 | 첫 화면에 북랩의 핵심 가치, 대표 수치, 상담 CTA, 패키지 추천 CTA를 배치한다. | P0 |
| H-02 | "출판 목적 선택" 진단 진입을 제공한다: 서점 유통, 소량 제작, 교재, 전자책, 청소년, 출판사 대행. | P0 |
| H-03 | 출간 종수, 세종도서 선정, POD센터, POS 판매 확인 등 신뢰 증거를 카드/수치로 보여준다. | P0 |
| H-04 | 대표 패키지 4-6개를 목적 중심으로 재분류하고 예상 비용/포함 서비스를 바로 비교한다. | P0 |
| H-05 | 실제 출간 도서, 후기, 보도/수상/서점 유통 사례를 홈에서 노출한다. | P1 |
| H-06 | 모든 주요 섹션 말미에 상담/견적/패키지 추천 CTA를 반복 제공한다. | P0 |

### 7.2 Publishing Journey Requirements

| ID | Requirement | Priority |
|---|---|---|
| J-01 | 출판 과정을 원고 접수, 상담/견적, 계약, 교정/디자인, 인쇄/POD, 유통/정산으로 재구성한다. | P0 |
| J-02 | 각 단계마다 고객이 준비할 것, 북랩이 해주는 것, 예상 산출물을 구분한다. | P0 |
| J-03 | 과정 페이지에서 패키지 추천 또는 상담 신청으로 이어지는 고정 CTA를 제공한다. | P1 |

### 7.3 Conversion Requirements

| ID | Requirement | Priority |
|---|---|---|
| C-01 | 상담 신청 폼은 목적, 원고 상태, 장르, 예상 부수, 연락처만으로 1차 제출 가능해야 한다. | P0 |
| C-02 | 폼 제출 전 "내게 맞는 패키지"를 예비 추천하고 상담 연결 문구를 제공한다. | P1 |
| C-03 | 전화, 카카오톡, 이메일, 원고 전송, 출간 신청의 차이를 명확히 안내한다. | P0 |
| C-04 | 모바일에서 상담 CTA가 항상 접근 가능해야 한다. | P0 |

### 7.4 Content Requirements

| ID | Requirement | Priority |
|---|---|---|
| T-01 | FAQ를 비용, 제작, 교정/디자인, 유통, 인세, 소량 제작으로 재분류한다. | P1 |
| T-02 | 후기/사례는 "초보 저자", "전문가 브랜딩", "소량 제작", "교재" 등 페르소나별로 묶는다. | P1 |
| T-03 | 기존 회사 연혁은 별도 페이지에 두되 홈에는 신뢰 수치만 압축 노출한다. | P1 |
| T-04 | 기존 패키지 상세 내용은 유지하되 비교표와 추천 진단으로 진입 장벽을 낮춘다. | P0 |

## 8. Success Metrics

### Primary Metrics

- 상담 신청 전환율: 현재 대비 +30% 이상
- 출간 신청/원고 전송 클릭률: 현재 대비 +20% 이상
- 패키지 상세 진입률: 홈 방문 대비 +25% 이상
- 모바일 상담 CTA 클릭률: 현재 대비 +30% 이상

### Secondary Metrics

- FAQ 페이지 이탈률 감소
- 패키지 선택 진단 완료율 40% 이상
- 상담 폼 시작 대비 제출 완료율 65% 이상
- 평균 상담 전 사전 정보 수집 항목 수 증가: 목적, 장르, 원고 상태, 부수 등

## 9. MVP Scope

### In Scope

- 홈 리뉴얼 정보 구조
- 상담 전환 CTA 체계
- 목적 기반 패키지 추천 UX
- 출판 과정/신뢰 증거/후기/FAQ 홈 섹션
- 모바일 우선 CTA 및 폼 UX
- 기존 콘텐츠를 재사용하는 IA 개편

### Out of Scope for MVP

- 실제 결제 시스템 개편
- MY북랩/POS 내부 기능 재개발
- 신규 CRM 구축
- 전체 서점/도서 DB 마이그레이션
- 앱 개발

## 10. Beachhead Segment and GTM

### Beachhead

가장 먼저 공략할 세그먼트는 "첫 책을 준비하는 개인 저자"다. 이유는 상담 전환 UX 개선 효과가 가장 크고, 비용/과정/신뢰에 대한 불안이 명확하며, 북랩의 패키지 상품과 가장 직접적으로 연결되기 때문이다.

### GTM Message

- Main: "내 원고에 맞는 출판 방법과 비용을 먼저 확인하세요."
- Support: "북랩은 패키지 비용, 자체 제작, 서점 유통, 판매 확인까지 한 번에 안내합니다."
- CTA: "무료 출판 상담 시작하기", "내 책 패키지 추천 받기"

## 11. Risks and Open Questions

| Risk / Question | Impact | Mitigation |
|---|---|---|
| 기존 사이트 CMS/레거시 구조가 최신 프론트엔드 구현을 제한할 수 있음 | High | Plan 단계에서 기술 스택과 배포 구조 확인 필요 |
| 가격/패키지 정보가 자주 변경될 경우 정적 콘텐츠 유지 비용 증가 | Medium | 패키지 데이터 소스 분리 또는 관리자 편집 구조 검토 |
| 좋은땅과 유사한 구성만 따라가면 북랩 고유성이 약해질 수 있음 | Medium | 패키지 투명성, POD 제작, POS 확인을 핵심 차별점으로 고정 |
| 상담 폼 항목을 늘리면 전환율이 떨어질 수 있음 | Medium | 1차 간편 제출 후 상세 정보는 후속 단계에서 수집 |
| 후기/사례 콘텐츠가 충분히 정리되어 있지 않을 수 있음 | Medium | MVP는 기존 출간 도서/수상/연혁으로 대체, 이후 후기 수집 |

## 12. Source Notes

- Booklab main/search cache: https://www.book.co.kr/
- Booklab package guide: https://www.book.co.kr/essay_ver2/publish/package_guide.php
- Booklab company page: https://www.book.co.kr/essay_ver2/company/company.php
- Booklab publishing guide: https://www.book.co.kr/essay_ver2/guide/print_guide.php
- G-World main: https://www.g-world.co.kr/
- G-World publishing process: https://www.g-world.co.kr/guide/process
- G-World consultation page: https://www.g-world.co.kr/counsel
- G-World guide page: https://www.g-world.co.kr/guide
- G-World marketing page: https://www.g-world.co.kr/guide/marketing
- Kyobo POD reference: https://product.kyobobook.co.kr/pod/main
- Bookk reference search result: https://www.besuccess.com/bookk-kyobo/
- U-Paper reference search result: https://www.etnews.com/201307220248

## 13. Next PDCA Step

Recommended next command:

```text
/pdca plan booklab-renewal
```

Plan 단계에서는 다음을 확정해야 한다.

- 현재 북랩 사이트의 기술 스택과 배포 방식
- 리뉴얼 범위: 홈만, 주요 랜딩까지, 또는 전체 IA 개편
- 상담 폼/CRM/원고 전송 기능의 실제 연동 범위
- 기존 콘텐츠 및 도서 DB 재사용 방식
- 디자인 방향: 북랩 브랜드 유지 vs 브랜드 톤 재정의
