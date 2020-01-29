exchange rate prediction

This project is to predict exchange rate using deep-learning.  
This model used usd/krw exchange rate.   

00. 통화량 변화율 정리 

1. 네이버 금융 뉴스 크롤링  
-> 추후 텍스트 마이닝 하기 위해서 네이버 금융 뉴스 top10 제목만 뽑음  
  
2. usd_krw_prediction(using LSTM, 10day prediction(using 10days data))  
-> RMSE : 0.0489, 테스트결과 실제 데이터에 따라가는 모습을 보임  

3. usd_krw_prediction(using LSTM, 1day prediction(using 1days data))  
-> RMSE : 0.0456, 테스트결과 실제 데이터에 비슷한 모습을 보임  
