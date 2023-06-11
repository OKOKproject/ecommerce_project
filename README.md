# ecommerce_project

깃헙 폴더 구조 어떻게 할건지 상의필요.

# 1주차 정리(06.07 ~ 06.11)

1. 이커머스(의류)와 관련된 것은 주어진 데이터셋을 활용하여 처리하면 기간이 딱 떨어지지 않는다면 문제가 발생할 수 있음 
  
    : 계절별 판매량이 다르기 때문
    - 기간을 최근 2년으로 처리하여 데이터를 확인하면 해결 가능
  
2. transation에서 session_id는 같지만 여러 row로 표시되어 총합을 계산하는 row들이 존재함

   : 세션으로 묶어서 한번의 주문으로 인식하도록 변경

3. 구매에 대한 기준 : 구매시도 or 구매완료
  - 구매 완료 기준으로 결정
 
    a. 구매 시도에서 구매완료로 이어지는 경우 95.7%로 높은 확률로 구매를 완료하여 데이터의 수가 차이가 별로 없음
    
    b. 기타 구매하는 기기의 종류, 계절, 결제 방식 등의 요인이 미세하지만 영향을 줄 수 있을 것이라고 판단함.
