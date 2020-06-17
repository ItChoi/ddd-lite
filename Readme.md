## DDD-Lite

### 도메인 설계

상품(Product)
- 상품의 이름이 존재한다.
- 상품의 가격이 있다.

주문(Order)
- 주문은 배송지 정보를 가진다.
- 주문은 주문 상태(결제 대기 중, 준비 중, 배송 중, 배송 완료, 결제 취소)를 가진다.
- 주문은 하나 이상의 주문 품목을 가진다.

주문 품목(OrderLine)
- 주문 품목은 주문 수량을 가진다.
- 주문 품목은 상품 정보를 가진다.

결제(Payment)
- 결제 정보는 여러 종류(신용카드, 모바일)가 사용 된다.

배송(Delivery)
- 배송은 배송 상태(배송 중, 배송 완료)를 가진다.

### 기능 요구사항

1. 고객이 상품을 주문한다.
2. 고객이 결제한다.
3. 결제가 완료되면 배송을 시작한다.
4. 고객은 주문을 취소할 수 있다.
5. 주문이 취소되면 배송이 취소된다.
6. 배송 상태가 배송 중이라면 결제를 취소할 수 없다.

### 구현 요구사항

- Event 개념 활용 (필수)
- Factory 개념 활용
- Repository 개념 활용 (필수)
- Service 개념 활용
- Value Object 개념 활용 (필수)
- Aggregate 개념 활용

위의 개념들을 적절히 사용하여 구현한다.