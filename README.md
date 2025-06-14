### 문제 정의
고객의 다양한 구매 및 재구매 행동을 기반으로 유형을 분류하고, 이를 통해 효율적인 쿠폰 분배 전략을 수립하고자 했습니다. 
쿠폰을 일괄적으로 제공하기보다는, 구매 전환 가능성이 높은 고객에게 선별적으로 제공하는 방식이 필요했습니다.

### 프로젝트 목적
- 고객 데이터를 기반으로 행동 및 특성 중심의 세분화 수행
- 각 고객 유형의 재구매율 및 구매 성향 분석
- 분석 결과를 바탕으로 합리적이고 전략적인 쿠폰 분배 기준 수립

### 분석 과정
#### 1. 데이터 구성 및 전처리
- 고객 ID, 상품 ID, 카테고리, 구매 이력 등을 사용
- 고객별 재구매율, 구매 상품 수, 구매 카테고리 수 등의 파생 변수 생성

#### 2. 클러스터링
- KMeans 클러스터링을 통해 고객을 5개 유형으로 분류
- 각 군집의 평균 재구매율, 구매 품목 수 등을 기반으로 고객 특성 해석

#### 3. 클러스터 해석
- 고재구매율 & 다양한 소비를 보이는 핵심 고객군
- 저구매율 & 단일 카테고리 소비에 집중된 잠재 이탈군 등 구분

### 쿠폰 분배 전략 수립
- 클러스터별 특성을 바탕으로 쿠폰 제공 여부를 전략적으로 결정
- 세그먼트 - 관심카테고리 조합을 타겟으로 설정
- 전환 기대값 (쿠폰 사용률 X 카테고리 평균 주문 금액)을 계산하여 사분위 구간별 할인율을 10%, 20%, 30%로 설정 


### 인사이트
- 단순한 전체 제공보다, 클러스터 기반 선별 발송이 자원 효율성과 마케팅 효과 모두에서 유리
- 고객의 재구매율과 소비 다양성은 반응 가능성을 예측하는 주요 지표로 활용 가능
- 데이터 기반 고객 세분화 → 전략적 쿠폰 분배라는 실무 연계 분석 흐름을 성공적으로 구성함
