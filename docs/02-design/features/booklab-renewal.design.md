# Design: Booklab Site Renewal Proposal

- Feature ID: `booklab-renewal`
- Date: 2026-05-18
- Phase: PDCA Design
- Upstream PRD: `docs/00-pm/booklab-renewal.prd.md`
- Upstream Plan: `docs/01-plan/features/booklab-renewal.plan.md`
- Target site: https://www.book.co.kr/
- Benchmark site: https://www.g-world.co.kr/
- Design Purpose: 북랩 홈페이지 리뉴얼 제안서 및 이후 프로토타입 제작 기준

## Context Anchor

| Anchor | 내용 |
|---|---|
| WHY | 정보 나열형 출판사 사이트를 상담 전환형 출판 플랫폼으로 바꿔 상담 문의와 출간 신청 전환을 높인다. |
| WHO | 첫 책을 준비하는 개인 저자, 전문가/강사 저자, 소량 제작이 필요한 단체/학교/가족 프로젝트 고객. |
| RISK | 기존 레거시 사이트/CMS 구조, 가격 정보 관리, 좋은땅과의 유사성, 상담 폼 항목 과다, 후기 콘텐츠 부족. |
| SUCCESS | 상담 신청 전환율 +30%, 출간 신청/원고 전송 클릭률 +20%, 패키지 상세 진입률 +25%, 모바일 CTA 클릭률 +30%. |
| SCOPE | MVP는 홈 리뉴얼, 상담 CTA 체계, 목적 기반 패키지 추천, 출판 과정/신뢰/후기/FAQ 섹션, 모바일 폼 UX까지 포함한다. 결제, MY북랩/POS 내부 재개발, 신규 CRM은 제외한다. |

## 1. Overview

### 1.1 Design Goal

이 Design 문서는 북랩 홈페이지를 좋은땅 홈페이지의 전환 구조를 벤치마킹해 리뉴얼하는 제안서와 프로토타입 제작 기준을 정의한다.

핵심은 좋은땅을 시각적으로 복제하는 것이 아니라, 좋은땅이 잘하고 있는 "상담 전환 구조, 신뢰 증거 배치, 출판 과정 안내, 저자 불안 해소 흐름"을 북랩의 고유 강점에 맞게 재구성하는 것이다.

### 1.2 Renewal Concept

| 항목 | 제안 방향 |
|---|---|
| 리뉴얼 콘셉트 | 내 원고에 맞는 출판 방법과 비용을 먼저 알려주는 상담형 출판 플랫폼 |
| 핵심 메시지 | "책을 내고 싶다면, 내 원고에 맞는 출판 방식부터 확인하세요." |
| 차별 메시지 | 패키지 가격, 자체 제작, 서점 유통, 판매 확인까지 투명하게 안내하는 북랩 |
| UX 전략 | 첫 화면에서 판단 근거를 주고, 목적 선택으로 패키지를 좁히고, 상담으로 연결한다. |
| 제안서 키워드 | 전환 중심, 신뢰 강화, 목적 기반 패키지 추천, 모바일 상담 최적화 |

## 2. Benchmark Diagnosis

### 2.1 Current Booklab vs G-World

| 비교 축 | 현재 북랩 방향 | 좋은땅 벤치마킹 포인트 | 북랩 리뉴얼 제안 |
|---|---|---|---|
| 첫 화면 | 출판 플랫폼/패키지 정보 중심 | 출판 상담 CTA와 신뢰 메시지가 명확함 | 히어로에 상담 CTA, 패키지 추천 CTA, 신뢰 수치를 함께 배치 |
| 상담 전환 | 여러 메뉴와 신청 경로가 분산될 수 있음 | "출판 상담하기"가 반복 노출됨 | 상담, 원고 전송, 견적, 패키지 추천을 역할별 CTA로 정리 |
| 출판 과정 | 정보는 있으나 여정형 설득이 약함 | 컨설팅부터 유통/마케팅까지 단계화 | "원고 접수부터 서점 유통까지" 6단계로 시각화 |
| 신뢰 증거 | 연혁/설비/선정 이력이 하위 정보로 분산 | 후기, 저자 콘텐츠, 정산/앱 가치 노출 | 출간종수, 세종도서, POD센터, POS 판매 확인을 홈으로 승격 |
| 패키지 탐색 | 상품 종류가 많아 초보자가 고르기 어려움 | 상담으로 빠르게 유도 | 목적 기반 4문항 추천으로 적합 패키지를 좁힘 |
| 사후 관리 | POS 판매 확인 기능의 가치가 약하게 보일 수 있음 | 인세/정산/현황 확인을 불안 해소 장치로 사용 | POS 판매 확인을 "출간 후에도 확인 가능한 북랩" 메시지로 재배치 |

### 2.2 Proposal Takeaway

제안서에는 다음 문장 구조를 사용한다.

> 좋은땅은 상담 전환과 신뢰 형성의 흐름이 강한 사이트입니다. 북랩은 여기에 더해 패키지 가격 투명성, POD 자체 제작, POS 판매 확인이라는 실질적 강점을 보유하고 있습니다. 따라서 이번 리뉴얼은 좋은땅의 전환 구조를 벤치마킹하되, 북랩만의 객관적 신뢰 자산을 전면에 배치하는 방향이 적합합니다.

## 3. Architecture Options

### 3.1 Option A: Static Renewal Prototype

정적 HTML/CSS/JS 또는 간단한 프론트엔드 앱으로 리뉴얼 홈 시안을 먼저 구현한다.

| 항목 | 내용 |
|---|---|
| 장점 | 제안서/미팅에서 바로 보여줄 수 있고 기존 시스템 제약을 받지 않는다. 화면 구성, 카피, CTA 흐름을 빠르게 검증할 수 있다. |
| 단점 | 실제 북랩 운영 시스템과 바로 연결되지는 않는다. 이후 CMS/서버 통합 설계가 별도로 필요하다. |
| 적합성 | 이번 목표가 "리뉴얼 제안서와 방향 제시"이므로 가장 적합하다. |

### 3.2 Option B: Existing CMS Integration

기존 북랩 사이트의 CMS 또는 템플릿 구조를 유지하면서 메인 콘텐츠 블록과 CTA를 개선한다.

| 항목 | 내용 |
|---|---|
| 장점 | 실제 운영 반영이 빠를 수 있고 기존 콘텐츠/회원/상담 시스템을 유지할 수 있다. |
| 단점 | 레거시 구조에 따라 디자인 자유도, 모바일 최적화, 상호작용 구현이 제한될 수 있다. |
| 적합성 | 기존 시스템 구조가 확인된 뒤 운영 반영 단계에서 검토한다. |

### 3.3 Option C: Modern Frontend Rebuild

Next.js 등 최신 프론트엔드로 홈, 패키지 추천, 상담 흐름을 재구축하고 기존 시스템과 연동한다.

| 항목 | 내용 |
|---|---|
| 장점 | 성능, 확장성, 콘텐츠 구조화, 추적 분석, A/B 테스트에 유리하다. |
| 단점 | 초기 개발 범위가 커지고 기존 시스템 연동 비용이 발생한다. |
| 적합성 | 리뉴얼이 홈 개선을 넘어 장기 플랫폼 개편으로 확장될 때 적합하다. |

### 3.4 Recommendation

| 기준 | Option A | Option B | Option C |
|---|---:|---:|---:|
| 제안서 설득력 | High | Medium | Medium |
| 구현 속도 | High | Medium | Low |
| 기존 시스템 의존도 | Low | High | Medium |
| 실제 운영 반영성 | Low | High | High |
| 장기 확장성 | Medium | Low | High |
| 리스크 | Low | Medium | High |

추천안은 **Option A: Static Renewal Prototype**이다.

이유는 이번 작업의 1차 목표가 "북랩 홈페이지가 이런 식으로 리뉴얼될 수 있다"는 제안서와 방향 제시이기 때문이다. 먼저 정적 프로토타입으로 메인 구조, 카피, CTA, 패키지 추천 흐름을 보여주고, 제안이 승인되면 기존 CMS 통합 또는 신규 프론트엔드 재구축으로 전환한다.

## 4. Information Architecture

### 4.1 Proposed Top Navigation

기존 북랩 GNB 구조를 유지하되, 리뉴얼에서는 이미지 탭 메뉴를 텍스트 기반 내비게이션으로 재구성한다. 메뉴명과 URL은 현재 사이트의 실제 구조를 기준으로 삼는다.

| 순서 | 기존 ID | 메뉴 | URL / 동작 | 리뉴얼 내 역할 | 비고 |
|---:|---|---|---|---|---|
| 1 | `gnb1` | 회사소개 | `/essay_ver2/company/company.php` | 북랩 신뢰와 회사 이력 확인 | 출간종수, 세종도서, POD 제작 역량 등 신뢰 근거와 연결 |
| 2 | `gnb2` | 출판가이드 | `/essay_ver2/guide/print_guide.php` | 출판 과정, 유통, 인세, 제작 절차 안내 | 좋은땅의 `출판 가이드` 벤치마킹 핵심 메뉴 |
| 3 | `gnb3` | 가격표 | `/essay_ver2/publish/service.php` | 패키지 비용과 기준 사양 확인 | 북랩의 차별점인 가격 투명성을 전면화 |
| 4 | `gnb4` | 출간문의 | `/essay_ver2/publish/advice.php` | 상담 전환의 핵심 메뉴 | 상단/메인/하단 CTA와 반복 연결 |
| 5 | `gnb5` | 인쇄/제본신청 | `/essay_ver2/shop/nonsalereqest.php` | 소량 제작, 비매품, 제본 신청 | 50부 프로젝트/개인 배포 니즈와 연결 |
| 6 | `gnb6` | 홍보/마케팅 | `/essay_ver2/promote/promote.php` | 출간 이후 홍보 지원 안내 | 좋은땅의 `마케팅 프로그램` 벤치마킹 대응 메뉴 |
| 7 | `gnb7` | 북스토어 | `movepage_href('7', '1', '', '')` | 출간 도서, 신간, 베스트셀러, 분야별 도서 탐색 | 좋은땅의 `책 소개`, `화제의 책`, `베스트셀러` 구조와 연결 |

리뉴얼 GNB 권장 표기:

```text
회사소개 | 출판가이드 | 가격표 | 출간문의 | 인쇄/제본신청 | 홍보/마케팅 | 북스토어
```

리뉴얼 시 우선순위는 `출간문의`를 가장 강한 CTA로 만들고, `가격표`, `출판가이드`, `북스토어`를 메인 콘텐츠와 반복 연결하는 것이다.

### 4.2 Homepage Section Order

아래 구성은 현재 북랩 메인 HTML에서 확인되는 실제 콘텐츠를 기준으로 정리한 것이다. 리뉴얼 제안에서는 기존 메인의 콘텐츠 자산을 유지하되, 좋은땅처럼 상담 전환과 도서/저자 콘텐츠가 더 잘 보이도록 재배치한다.

| 순서 | 현재 메인 섹션 | 현재 포함 콘텐츠 | 리뉴얼 방향 | 주요 연결 |
|---:|---|---|---|---|
| 1 | 메인 비주얼 배너 | `출간문의`, `인세 받는 즐거움`, `책 판매부수 공개` 배너 슬라이드 | 첫 화면에서 출간문의, 인세/판매 확인, 상담 CTA가 바로 보이도록 유지 및 강화 | `/essay_ver2/publish/advice.php`, `/essay_ver2/publish/package.php`, `/essay_ver2/guide/sell.php` |
| 2 | 출판 서비스 3대 배너 | `출판유통`, `출판도구 모음`, `인쇄 및 제본` | 북랩이 제공하는 서비스 범위를 한눈에 보여주는 핵심 안내 영역으로 유지 | 출판유통 방식, 원고전송, 셀프견적, 프로필 생성기, 페이지 계산기, 인쇄/제본 주문 |
| 3 | 명예의 전당 | 세종도서, 국방부 진중문고 등 선정 도서와 대표 도서 표지 | 북랩의 가장 강한 신뢰 근거로 상단 주요 섹션화 | `/essay_ver2/bshop/index.php?grp=fame` |
| 4 | 북스토어 / 신간도서 | 추천 도서, 신간 도서, 도서 표지, 도서명 | 좋은땅의 `책 소개`, `화제의 책`, `베스트셀러`처럼 도서 탐색 중심 섹션으로 확장 | `/essay_ver2/bshop/index.php` |
| 5 | 작가 셀프 인터뷰 | 작가 사진, 작가명, 도서명, 인터뷰 요약 | 저자 후기/인터뷰 신뢰 콘텐츠로 유지하고 가독성 개선 | `/essay_ver2/promote/interview_list.php` |
| 6 | 북랩 NEWS | 무이자 할부, 인세지급 안내, 공지사항 | 운영 신뢰와 최신 공지를 보여주는 보조 정보 영역으로 유지 | `/essay_ver2/bbs/list.php?code=booklab_news` |
| 7 | 북랩 Story | 출간 종수 8천 종 돌파, 교보문고 진열 등 사진 뉴스 | 북랩의 성과와 유통 사례를 보여주는 신뢰 콘텐츠로 강화 | `/essay_ver2/bbs/list.php?code=photo` |
| 8 | 상담/결제 안내 | 상담전화, 신용카드 결제, 무통장입금 안내 | 문의 전환과 결제 신뢰 정보를 한 영역에 정리 | `/essay_ver2/support/tel_info.php`, 신용카드 결제, `/essay_ver2/support/bankbook.php` |
| 9 | 하단 빠른 메뉴 | 원고전송, 원고정서 가이드, 나의 출판계약서, 내 책 홍보하기 | 저자 작업 도구 바로가기 영역으로 유지 | 원고전송, `/essay_ver2/guide/model.php`, `/essay_ver2/mypage/contract_list.php`, `/essay_ver2/mypage/mail_pr_product.php` |
| 10 | 하단 빠른 메뉴 2열 | 출판가이드북, 무료 본문 템플릿, 도서유통망, 도서판매량 및 인세 | 출판 준비/유통/판매 확인 도구 영역으로 재정리 | 출판가이드북, 블로그, `/essay_ver2/company/intro_bookstore.php`, `/essay_ver2/mypage/sales_sales_royalty.php` |
| 11 | 우측 퀵 메뉴 | 원고전송, 신용카드 결제, 무이자 할부, 저자구매, 현금영수증, 배송조회, 도서목록 다운로드 등 | 좋은땅의 상담/저자 도구 접근성을 참고해 플로팅 유틸 메뉴로 정리 | 원고전송, 결제, 배송조회, 저자구매, 도서목록 다운로드 |
| 12 | 푸터 | 회사소개, 오시는 길, 회원가입, 약관, 개인정보, 인재채용, 고객센터, 블로그, 회사 정보 | 기존 법적/회사 정보 유지 | 회사소개, 고객센터, 블로그, 회사 정보 |

현재 메인에서 반드시 유지해야 할 콘텐츠 축:

```text
메인 배너 / 출판 서비스 3대 배너 / 명예의 전당 / 북스토어 / 작가 인터뷰 / 북랩 NEWS / 북랩 Story / 상담·결제 안내 / 저자용 빠른 메뉴 / 우측 퀵 메뉴
```

좋은땅 벤치마킹은 이 콘텐츠를 대체하는 것이 아니라, 기존 콘텐츠를 더 잘 보이게 재배치하는 기준으로 사용한다. 특히 `출간문의`, `작가 인터뷰`, `책 소개`, `판매/인세 확인`, `마케팅/홍보` 흐름은 좋은땅과 비교해 제안서에서 직접 설명할 수 있는 항목이다.

## 5. UX Design Specification

### 5.1 Hero Section

제안 카피:

- Headline: `내 원고에 맞는 출판 방법과 비용을 먼저 확인하세요`
- Subcopy: `북랩은 패키지 비용, 자체 제작, 서점 유통, 판매 확인까지 한 번에 안내하는 출판 파트너입니다.`
- Primary CTA: `무료 출판 상담 시작하기`
- Secondary CTA: `내 책 패키지 추천 받기`

구성:

- 왼쪽: 핵심 카피, CTA 2개, 신뢰 수치 3개
- 오른쪽: 출간 도서 이미지/책 목업/상담 프로세스 미니 카드
- 모바일: 카피, CTA, 신뢰 수치, 대표 책 이미지 순서

### 5.2 Trust Metrics

| 항목 | 메시지 방향 |
|---|---|
| 출간종수 | "8천 종 이상 출간 경험" 형태로 누적 경험 강조 |
| 세종도서 | "공신력 있는 선정 이력"으로 품질 신뢰 강화 |
| POD센터 | "자체 제작 기반의 안정적인 제작 관리" 강조 |
| POS 판매 확인 | "출간 후 판매 현황까지 확인 가능한 사후 관리" 강조 |

### 5.3 Purpose Selector

사용자는 패키지명을 먼저 보는 대신 자신의 목적을 선택한다.

| 목적 | 연결 메시지 |
|---|---|
| 서점 유통을 하고 싶어요 | 정식 출간과 온라인/오프라인 유통 중심 안내 |
| 적은 부수만 만들고 싶어요 | 50부 프로젝트/소량 제작 안내 |
| 교재나 강의 책을 만들고 싶어요 | 교재/전문서 패키지 안내 |
| 전자책으로 먼저 내고 싶어요 | 전자책 출판 옵션 안내 |
| 청소년 저자입니다 | 청소년 맞춤 패키지 안내 |
| 출판사 운영 대행이 필요해요 | 출판사 대행/위탁 운영 안내 |

### 5.4 Package Recommendation Flow

질문은 4개 이하로 제한한다.

1. 어떤 목적으로 책을 내고 싶나요?
2. 원고는 어느 정도 준비되어 있나요?
3. 몇 부 정도 필요하신가요?
4. 서점 유통이 필요하신가요?

결과 화면:

- 추천 패키지명
- 추천 이유 2-3줄
- 포함 가능 서비스
- 예상 비용 확인 또는 상담 CTA
- 기존 상세 페이지 연결

### 5.5 Publishing Journey

6단계 구조:

| 단계 | 고객이 하는 일 | 북랩이 하는 일 |
|---|---|---|
| 1. 원고 접수 | 원고/기획 의도 전달 | 원고 상태와 출판 목적 확인 |
| 2. 상담/견적 | 희망 사양, 부수, 유통 여부 선택 | 적합 패키지와 예상 비용 안내 |
| 3. 계약 | 출판 조건 확인 | 일정, 제작 범위, 유통 조건 확정 |
| 4. 교정/디자인 | 수정 의견 확인 | 교정, 편집, 표지/본문 디자인 진행 |
| 5. 인쇄/POD | 최종본 승인 | 자체 제작/POD 기반 인쇄 진행 |
| 6. 유통/정산 | 판매 현황 확인 | 서점 유통, POS 판매 확인, 정산 안내 |

### 5.6 Mobile Conversion

모바일 하단 고정 CTA:

- Primary: `상담`
- Secondary: `추천`
- Optional: `전화`

모바일 원칙:

- 첫 화면에서 CTA 2개가 보여야 한다.
- 패키지 추천은 한 화면에 한 질문씩 보여준다.
- 긴 비교표는 카드형으로 전환한다.
- 상담 폼은 1차 제출 기준 5개 이하 필드로 제한한다.

## 6. Proposal Slide Structure

제안서로 확장할 때는 다음 구성을 권장한다.

| 슬라이드 | 제목 | 핵심 내용 |
|---:|---|---|
| 1 | 북랩 홈페이지 리뉴얼 제안 | 프로젝트 목적과 한 줄 방향 |
| 2 | 현재 사이트 진단 | 정보 분산, CTA 약화, 신뢰 증거 노출 부족 |
| 3 | 좋은땅 벤치마킹 인사이트 | 상담 전환, 과정 안내, 후기/신뢰 구조 |
| 4 | 리뉴얼 전략 | 좋은땅의 구조 + 북랩의 차별 자산 |
| 5 | 메인 화면 구성안 | 홈 섹션 순서와 사용자 흐름 |
| 6 | 핵심 기능 1: 상담 전환 | CTA 체계와 모바일 고정 CTA |
| 7 | 핵심 기능 2: 패키지 추천 | 목적 기반 4문항 추천 UX |
| 8 | 핵심 기능 3: 신뢰 강화 | 출간종수, POD, POS, 세종도서 |
| 9 | 기대 효과 | 상담 전환율, 패키지 진입률, 모바일 전환 개선 |
| 10 | 추진 단계 | 프로토타입, 검토, 실제 적용, 고도화 |

## 7. Component Design

### 7.1 Component Map

| Component | Role | Required Data |
|---|---|---|
| `HeroSection` | 첫 화면 가치 제안과 CTA | headline, subcopy, metrics, CTA URLs |
| `TrustMetrics` | 객관적 신뢰 증거 | metric label, value, description |
| `PurposeSelector` | 사용자의 출판 목적 선택 | purpose list, icon, copy |
| `PackageRecommender` | 4문항 추천 플로우 | question set, package mapping |
| `PackageComparison` | 대표 패키지 비교 | package name, purpose, spec, price/cost CTA |
| `PublishingJourney` | 출판 과정 6단계 안내 | step title, customer action, Booklab action |
| `BooklabDifference` | 북랩 차별점 설명 | POD, POS, cost transparency, distribution |
| `CaseShowcase` | 출간 도서/후기 | book title, cover, author/comment |
| `FAQAccordion` | 불안 해소 질문 | category, question, answer |
| `ConsultationCTA` | 상담 전환 | CTA label, channel, form URL |
| `MobileStickyCTA` | 모바일 상시 전환 | 상담/추천/전화 action |

### 7.2 Data Model for Prototype

```ts
type Metric = {
  label: string;
  value: string;
  description: string;
};

type Purpose = {
  id: string;
  label: string;
  description: string;
  recommendedPackages: string[];
};

type PackageItem = {
  id: string;
  name: string;
  target: string;
  bestFor: string;
  specs: string[];
  priceLabel: string;
  detailUrl?: string;
};

type RecommendationAnswer = {
  purpose: string;
  manuscriptStatus: string;
  quantity: string;
  distribution: string;
};

type JourneyStep = {
  title: string;
  customerAction: string;
  booklabAction: string;
};
```

## 8. Interaction Design

### 8.1 Package Recommendation Logic

| 조건 | 추천 방향 |
|---|---|
| 서점 유통 필요 + 초고 완료 | 정식 출판 패키지 상담 |
| 소량 제작 + 개인 배포 | 50부 프로젝트/소량 제작 |
| 교재/강의 목적 | 교재 패키지 |
| 전자책 우선 | 전자책 패키지 |
| 청소년 저자 | 청소년 출판 패키지 |
| 출판사 대행 | 출판사 대행 서비스 |

추천 결과는 확정 견적이 아니라 "상담 전 예비 추천"으로 표현한다. 가격 정보가 민감하거나 변경 가능하면 `예상 비용 확인하기` CTA로 연결한다.

### 8.2 CTA Rules

| 위치 | Primary CTA | Secondary CTA |
|---|---|---|
| Hero | 무료 출판 상담 시작하기 | 내 책 패키지 추천 받기 |
| Purpose Selector | 내 목적 선택하기 | 패키지 전체 보기 |
| Recommendation Result | 이 패키지로 상담하기 | 상세 보기 |
| Journey Section | 출판 과정 상담받기 | 준비 자료 보기 |
| Trust Section | 북랩 상담 시작하기 | 제작/유통 보기 |
| Final CTA | 무료 출판 상담 시작하기 | 원고 전송하기 |

## 9. Visual Direction

### 9.1 Tone

- 신뢰감 있는 출판사
- 복잡한 정보를 쉽게 안내하는 상담형 서비스
- 가격과 제작 과정을 투명하게 보여주는 실무형 브랜드
- 너무 감성적인 문예지 톤보다 명확하고 안정적인 출판 파트너 톤

### 9.2 Visual Principles

- 실제 책, 표지, 제작 과정, 상담 흐름이 보이는 이미지 사용
- 카드 남발보다 정보 위계가 분명한 섹션형 레이아웃 사용
- 신뢰 수치는 크게, 설명은 짧게
- 패키지 비교는 표보다 카드+핵심 사양 중심으로 모바일 대응
- CTA는 반복하되 같은 문구만 반복하지 않고 맥락별로 조정

### 9.3 Suggested Color Direction

| Token | Direction |
|---|---|
| Primary | 북랩 기존 브랜드와 맞는 선명한 블루 계열 |
| Accent | 상담/전환을 강조하는 따뜻한 포인트 컬러 |
| Neutral | 흰색, 연회색, 차분한 짙은 텍스트 |
| Trust | 신뢰 수치와 인증 요소에 사용하는 절제된 녹색 또는 딥 블루 |

정확한 색상 값은 실제 북랩 로고와 기존 브랜드 가이드를 확인한 뒤 Design Anchor 단계에서 확정한다.

## 10. Accessibility and Responsive Design

| 항목 | 기준 |
|---|---|
| Mobile first CTA | 모바일 하단 고정 CTA는 화면을 가리지 않고 안전 영역을 고려한다. |
| Text hierarchy | 히어로 외 섹션 제목은 과도하게 크지 않게 유지한다. |
| Touch target | 모바일 CTA와 선택 버튼은 최소 44px 높이를 확보한다. |
| Contrast | 본문/버튼 텍스트는 충분한 명도 대비를 가진다. |
| Form usability | 입력 필드는 자동완성, 전화번호 키패드, 명확한 오류 메시지를 제공한다. |

## 11. Test Plan

### 11.1 Static Review

| ID | Test | Expected |
|---|---|---|
| T-01 | 첫 화면 확인 | 핵심 카피, 신뢰 수치, 상담 CTA, 패키지 추천 CTA가 보인다. |
| T-02 | 벤치마킹 반영 확인 | 상담 전환, 과정 안내, 신뢰 구조가 좋은땅식 흐름으로 반영된다. |
| T-03 | 북랩 차별화 확인 | 가격 투명성, POD, POS, 출간 이력이 홈에서 확인된다. |
| T-04 | 제안서 활용성 확인 | 현황 진단, 벤치마킹, 리뉴얼 전략, 기대 효과 문구가 추출 가능하다. |

### 11.2 Interaction Review

| ID | Test | Expected |
|---|---|---|
| T-05 | 패키지 추천 플로우 | 4문항 이하로 추천 결과에 도달한다. |
| T-06 | CTA 흐름 | Hero, 추천 결과, 과정, FAQ, Final CTA가 상담으로 연결된다. |
| T-07 | 모바일 CTA | 모바일에서 상담/추천 CTA가 항상 접근 가능하다. |

### 11.3 Content Review

| ID | Test | Expected |
|---|---|---|
| T-08 | 패키지 비교 | 대표 패키지 4개 이상이 목적 중심으로 비교된다. |
| T-09 | FAQ | 비용, 제작, 유통, 정산, 소량 제작 질문이 포함된다. |
| T-10 | 출판 과정 | 6단계와 고객/북랩 역할이 구분된다. |

## 12. Implementation Guide

### 12.1 Recommended Implementation Path

1. 정적 프로토타입 또는 프론트엔드 목업으로 홈 1페이지를 만든다.
2. 제안서에 사용할 스크린샷과 섹션 설명을 확보한다.
3. 이해관계자 검토 후 실제 운영 반영 방식을 결정한다.
4. 기존 CMS 통합 또는 신규 프론트엔드 재구축 범위를 확정한다.
5. 상담 폼/원고 전송/기존 패키지 상세 URL 연결을 실제 환경에 맞게 조정한다.

### 12.2 File Plan for Prototype

현재 워크스페이스에는 앱 코드가 없으므로, 다음 단계(`/pdca do`)에서는 정적 프로토타입 기준으로 시작하는 것을 권장한다.

| File | Purpose |
|---|---|
| `prototype/booklab-renewal/index.html` | 제안서용 리뉴얼 홈 프로토타입 |
| `prototype/booklab-renewal/styles.css` | 반응형 레이아웃, 브랜드 톤, CTA 스타일 |
| `prototype/booklab-renewal/app.js` | 패키지 추천 인터랙션, FAQ 토글 |
| `prototype/booklab-renewal/assets/` | 책 표지/목업/이미지 자산 |

### 12.3 Session Guide

| Module | Scope | Output |
|---|---|---|
| module-1 | 제안서용 홈 구조와 카피 | `index.html` 섹션 구조, 핵심 카피 |
| module-2 | 스타일 및 반응형 UI | `styles.css`, 데스크톱/모바일 레이아웃 |
| module-3 | 패키지 추천/FAQ 인터랙션 | `app.js`, 추천 결과/FAQ 토글 |
| module-4 | 제안서 보조 문서 | 리뉴얼 제안서 목차/슬라이드 원고 |

추천 세션:

```text
/pdca do booklab-renewal --scope module-1,module-2
```

첫 구현은 제안서에 바로 캡처 가능한 정적 홈 프로토타입부터 만드는 것이 좋다. 이후 `module-3`으로 패키지 추천 인터랙션을 붙이고, 마지막에 `module-4`로 제안서 원고를 정리한다.

## 13. Decision Record

| Decision | Rationale |
|---|---|
| 좋은땅은 구조 벤치마크로 사용하고 시각/브랜드는 북랩 중심으로 재해석한다. | 단순 모방 리스크를 줄이고 북랩의 고유 강점을 전면화하기 위해서다. |
| 1차 산출물은 정적 리뉴얼 프로토타입으로 한다. | 제안서 목적상 빠르게 보여주고 피드백받는 것이 중요하다. |
| 패키지 탐색은 상품명보다 목적 선택을 우선한다. | 첫 책 저자와 초보 고객은 패키지명보다 자신의 상황에서 출발해야 이해가 쉽다. |
| 상담 폼은 최소 입력으로 설계한다. | 전환율 저하를 막고 상세 정보는 후속 상담에서 수집하기 위해서다. |
| POS 판매 확인과 POD 제작은 홈 신뢰 섹션에 포함한다. | 좋은땅 대비 북랩만의 객관적 차별 자산이기 때문이다. |

## 14. Next Step

다음 PDCA 단계:

```text
/pdca do booklab-renewal --scope module-1,module-2
```

구현 전에 다음 중 어느 산출물을 먼저 만들지 확정하면 된다.

1. 제안서에 넣을 정적 홈페이지 프로토타입
2. 제안서 문서/슬라이드 원고
3. 프로토타입과 제안서 원고를 함께 작성
