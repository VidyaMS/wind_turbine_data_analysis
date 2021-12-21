# wind_turbine_data_analysis

Data source : https://www.kaggle.com/berkerisen/wind-turbine-scada-dataset.   
  
Data Analysis Objective:  

Wind turbine data for a year starting from Jan 2018 to Dec 2018 is given . Data is at a frequncy of 10 mins interval.Wind speed, Power generated and wind direction are the variables along with the date.  

1. Analyse the data to understand how much wind speed is received at the turbine, how much power is generated , any dependency of wind speed on time of the year , any relation between wind speed and power generated etc ??
2. Using different models like ARIMA , or Neural Network like LSTM predict wind speed and power generated. 
  
Results : 

Using a simple four neuron LSTM , wind speed could be predicted with 92% accuracy as shown below.  

![wind_speed](https://user-images.githubusercontent.com/20832632/146923546-1ddaf10b-8047-4805-8faa-177bb459bdfa.png)

For predicting power generated, the data had to be resampled at 20 m ins interval and the four neuron LSTM could give 86% accuracy.  

![power_predict](https://user-images.githubusercontent.com/20832632/146923840-219c6605-441e-4133-b3dc-a0e884af56e1.png)

Future scope:    
1. By adding feature of wind direction , can we improve the prediction models ?  
2. Can we improve the models by including any external data such as geospatial data ??
