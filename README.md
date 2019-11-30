# 키친포스

## 요구 사항
- 간단한 치킨집 포스기를 구현한다.

- 메뉴 그룹
  - [ ] 메뉴 그룹을 등록할 수 있다.
    - [ ] 이름을 가진다.
  - [ ] 등록된 모든 메뉴 그룹을 조회할 수 있다.

- 메뉴
  - [ ] 메뉴를 등록할 수 있다. 
    - [ ] 이름을 가진다. 
    - [ ] 가격을 가진다.
      - [ ] 가격은 0원 이상이어야 한다.
    - [ ] 메뉴 그룹의 식별자를 가진다.
      - [ ] 메뉴 그룹이 존재해야 한다.
    - [ ] 여러 개의 메뉴 상품을 가진다.
      - [ ] 각각의 메뉴 상품에 대한 상품이 존재해야 한다.
      - [ ] 각각의 메뉴 상품의 가격의 합은 메뉴의 가격보다 크거나 같아야 한다.
        - [ ] 메뉴 상품의 가격 = 상품의 가격 * 메뉴 상품의 수량
    - [ ] 메뉴가 등록된 후에 메뉴 상품이 등록된다.
  - [ ] 등록된 모든 메뉴를 조회할 수 있다.
    - [ ] 메뉴에 등록된 메뉴 상품도 같이 조회할 수 있다.

- 메뉴 상품
  - [ ] 메뉴의 식별자를 가진다.
    - [ ] 메뉴가 미리 등록되어 있어야 한다.
  - [ ] 상품의 식별자를 가진다.
  - [ ] 수량을 가진다.

- 상품
  - [ ] 상품을 등록할 수 있다. 
    - [ ] 이름을 가진다. 
    - [ ] 가격을 가진다.
      - [ ] 가격은 0원 이상이어야 한다.
  - [ ] 등록된 모든 상품을 조회할 수 있다.

- 주문
  - [ ] 주문을 등록할 수 있다.
    - [ ] 주문 테이블의 식별자를 가진다.
      - [ ] 주문 테이블이 존재해야 한다.
      - [ ] 주문 테이블이 비어있을 수 없다.
    - [ ] 상태를 가진다.
      - [ ] '요리 중', '식사 중', '완료' 상태를 가질 수 있다.
      - [ ] 주문 등록 시 '요리 중' 상태가 된다.
    - [ ] 주문 시간을 가진다.
    - [ ] 여러 개의 주문 항목을 가진다.
      - [ ] 주문 항목은 비어있을 수 없다.
    - [ ] 주문 테이블의 그룹이 존재할 수 있다.
      - [ ] 존재한다면 테이블 그룹에 포함된 주문 테이블 중 가장 먼저 등록된 주문 테이블의 주문을 진행한다.
  - [ ] 등록된 모든 주문을 조회할 수 있다.
    - [ ] 주문에 등록된 주문 항목도 같이 조회할 수 있다.
  - [ ] 주문 상태를 변경할 수 있다.
    - [ ] 주문이 존재해야 한다.
    - [ ] 현재 주문의 상태가 '완료' 외의 상태여야 한다.

- 주문 항목
  - [ ] 주문의 식별자를 가진다.
  - [ ] 메뉴의 식별자를 가진다.
  - [ ] 수량을 가진다.

- 테이블 그룹
  - [ ] 테이블 그룹을 등록할 수 있다.
    - [ ] 생성 시간을 가진다. 
    - [ ] 여러 개의 주문 테이블을 가진다.
      - [ ] 주문 테이블은 2개 이상이어야 한다.
      - [ ] 주문 테이블은 비어있거나 다른 테이블 그룹에 포함되어 있지 않아야 한다.
    - [ ] 테이블 그룹 등록 시 주문 테이블은 등록된 테이블 그룹에 포함된다.
  - [ ] 테이블 그룹을 지울 수 있다.
    - [ ] 주문 테이블이 존재해야 한다.
    - [ ] 주문 테이블이 테이블 그룹에 포함되어 있어야 한다.
    - [ ] 주문 테이블의 주문은 '요리 중' 이거나 '식사 중'의 상태를 가질 수 없다.
    - [ ] 테이블 그룹 제거 시 주문 테이블은 테이블 그룹에서 제외된다.

- 주문 테이블
  - [ ] 주문 테이블을 등록할 수 있다.
    - [ ] 테이블 그룹의 식별자를 가진다.
    - [ ] 고객의 인원 수를 가진다.
    - [ ] 테이블이 비어있는 지의 여부를 가진다.
  - [ ] 등록된 모든 주문 테이블을 조회할 수 있다. 
  - [ ] 주문 테이블의 비어있음 여부를 변경할 수 있다.
    - [ ] 주문 테이블이 존재해야 한다.
    - [ ] 주문 테이블의 테이블 그룹이 없어야 한다.
    - [ ] 주문 테이블의 주문은 '요리 중' 이거나 '식사 중'의 상태를 가질 수 없다.
  - [ ] 주문 테이블의 고객의 인원 수를 변경할 수 있다.
    - [ ] 변경하려는 고객의 인원 수는 0명 이상이어야 한다.
    - [ ] 주문 테이블이 존재해야 한다.
    - [ ] 기존의 주문 테이블이 비어있을 수 없다.

## 용어 사전

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |

## 모델링

- 
