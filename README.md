exchange rate prediction

This project is to predict exchange rate using deep-learning.  
This model used usd/krw exchange rate.   

00. 통화량 변화율 정리 

 --------------------------------------

1. 네이버 금융 뉴스 크롤링  
-> 추후 텍스트 마이닝 하기 위해서 네이버 금융 뉴스 top10 제목만 뽑음  
  
  ------------------
  
2. usd_krw_prediction(using LSTM, 10day prediction(using 10days data))  
-> RMSE : 0.0489, 테스트결과 실제 데이터에 따라가는 모습을 보임  

3. usd_krw_prediction(using LSTM, 1day prediction(using 1days data))  
-> RMSE : 0.0456, 테스트결과 실제 데이터에 비슷한 모습을 보임  

----------------------

4. usd_krw_prediction(facebook prophet)    
-> 환율 데이터중 2019년의 데이터를 이용하여 2020년 1월을 예측함.   
-> holiday는 주말과 공휴일로 잡고, 파라미터를 수정하지 않은 상태에서는    
그래프의 모양이 단순 추세만 보이고 있다. 또한 주기성은 전혀 보이지 않음.    
-> 계속 파라미터를 수정하면서 해보려고 함.    
-> 계획 :  다른 기간으로 이용면 마지막 그래프 중에서 weekly를 이용할 수 있으므로   
이를 weekly를 주중만 나오게 설정하고 파라미터 수정하는 식으로 갈 예정.   


5. usd_krw_prediction(facebook prophet)  
-> 4번과 같은 데이터로 구성함.
-> 파라미터를 수정하고 실제 값과 예측값을 비교함  
-> 이와 유사하여 다양한 데이터셋을 나누어 실험을 해봄  
-> 총 10개의 데이터셋으로 한 결과 한개의 셋에서는 크게 보일지라도 스케일을 조정하면서 한다면 나쁘지않은 모델임을 확인할 수 있다.  
-> 이와 유사하게 스케일을 조정하여 6번에서 실험할 예정
