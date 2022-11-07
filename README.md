# Flight price prediction

![alt-text](https://github.com/HitPant/Flight_price_prediction/blob/main/images/flight_img.jpg)

This is my take on the the flight prediction problem.

### **Aim:** 
The problem aims at predicting the flight prices based on the following parameters:
1. Date_of_Journey
2. Source
3. Destination	
4. Route	
5. Dep_Time	(Departure time)
6. Arrival_Time	
7. Duration	
8. Total_Stops

**Model used:** RandomForest Regressor

### Following steps have been performed:

1. **Data description**
2. **EDA**
3. **Handling Object datatype**<br>
&nbsp;&nbsp;Date_of_Journey is an object data type<br>
&nbsp;&nbsp;to use this column for prediction we need to convert this datatype into timestamp<br>

![alt-text](https://github.com/HitPant/Flight_price_prediction/blob/main/images/cls.jpg)

&nbsp;&nbsp;**.dt.day** method will extract day of that date.<br>
&nbsp;&nbsp;**.dt.month** method will extract month of that date.

Similarly, for departure time we will use:<br>
**.dt.hour** and **.dt.minute** to separately extract the (hh : mm)

4. **Handling Categorical Data:**
&nbsp;&nbsp; We have 2 types of categorical variables in the dataset and following encoding have been performed:
&nbsp;&nbsp;&nbsp;Nominal data --> data are not in any order --> OneHotEncoder
&nbsp;&nbsp;&nbsp;Ordinal data --> data are in order --> LabelEncoder

5. **Comparing categorical var with price column:**
### Airline vs Price:
![alt-text](https://github.com/HitPant/Flight_price_prediction/blob/main/images/avsp.jpg)

### Source vs Price:
![alt-text](https://github.com/HitPant/Flight_price_prediction/blob/main/images/svsp.jpg)

6. **For Total_Stops** column we perform LabelEncoding

7. **Feature Selection:**
&nbsp;&nbsp;&nbsp;heatmap:
&nbsp;&nbsp;&nbsp;feature selection : ExtraTreeRegressor:

8. **Train Model:** RandomForestRegressor
9. **Hyperparameter Tuining**
10. Save model
