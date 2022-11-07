# Flight price prediction

![alt-text](https://github.com/HitPant/Flight_price_prediction/blob/main/images/flight_img.jpg)

This is my take on the the flight prediction problem.

### **Aim:** 
The problem aims at predicting the flight prices based on the following parameters:
1. Date_of_Journey
2. Source
3. Destination	
4. Route	
5. Dep_Time	
6. Arrival_Time	
7. Duration	
8. Total_Stops


### Following steps have been performed:

1. Data description
2. EDA
3. Handling Object datatype<br>
&nbsp;&nbsp;Date_of_Journey is an object data type<br>
&nbsp;&nbsp;to use this column for prediction we need to convert this datatype into timestamp<br>

![alt-text](https://github.com/HitPant/Flight_price_prediction/blob/main/images/cls.jpg)

&nbsp;&nbsp;.dt.day method will extract day of that date.
&nbsp;&nbsp;.dt.month method will extract month of that date.
