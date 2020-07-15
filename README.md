# ibmhc2020

### Link to presentation video: 
https://youtu.be/DAdhehKGWsU

source code and output on projects

Note:
Through out the project, we chose Pune City's City Bus as example.


For understanding demands and requirements, we contacted with the planning authorities of PMPML City Bus. 

## Forecast 
pause at 2:45 - there is a drop in demand by 70% to 80%  

This demand is gradually increassing. 

pause at 2:55 - we forecasted the increasing demand to predict the future loads. 
 

## dummy data 

We generated the dummy data from 15-02-2020 to 24-06-2020 
Load Data based on the demand drop value provided at "transitapp.com/covid" and the Forecasted rise in demand 




## Frequency and Timetable formation

here we have used two most widely used methods for determining the frequency of service.

built the timetabls with considering maximum bus occupancy at 35 passengers in a bus.


## deficit function 

Deficit Function gives clear understanding of number of buses at each stop throughout the operations. 

It provides the number of buses required to execute the timetable.

| File Name                 | Discription             | 
|---------------------------|:-----------------------:|
| routes.csv                |contains data about existing routes|
| beforeCovid dummy data.py | Python Script used for generate dummy data before lockdown |
| dummy data.py             | Python Script used for generate dummy data after lockdown | 
| dummy data.zip            |contains load data from 15-02-2020 to 24-02-2020 |
| JSON values extraction.py | Python Script to retrive the demand drop values form JSON file at "https://transitapp.com/coronavirus"|
| forecast.py               |Forecasts change in demand after lockdown|
| face_bustand.py           |Detects passengers waiting for bus and counts their waiting time |
| frequency and timetable.py|Script for genetating timetables from loads and routes.csv|
| timetable1.csv            |timetable generated by frequency method 1|
| timetable2.csv            |timetable generated by frequency method 1|
| Deficit function.py       |Determines the total fleet required for implimenting the timetable|
