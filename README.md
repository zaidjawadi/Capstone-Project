README

**Fuel consumption of different car models in Canada**


## Project Overview:


The Problem Area:
This project aims to explore the relationships between fuel consumption and CO2 emissions across different car models in Canada. This would allow comparison of fuel efficiency across different car makes and models and investigate how fuel efficiency has evolved from 1995 to 2023. With rising gas prices and increasing evidence of climate change and global warming, driven in part by increasing carbon emissions, fuel efficiency is an important consideration when purchasing a vehicle. Considering that the average person would change vehicles multiple times in a lifetime, and vehicles are a major investment and gas is a major expenditure, it is of interest to know and compare the consumption of the different vehicles available in the Canadian market.

The User:
Different drivers have different needs, and this study would help users compare gas consumption based on different criteria such as car make, model, engine size, or vehicle class.

The Big Idea:
Following a search, regression modeling has previously been performed on this problem. A model can be developed to predict future gas consumption for a potential car model based on features of a car as well as forecasting future carbon emissions. As data is updated by Government of Canada annually, it is possible to forecast future fuel consumption using a model that is built with car data from 1995 – 2023. 

The Impact:
One can see how technology has advanced over the years in terms of vehicle fuel consumption for the different car models and features. 
A comparison of fuel consumption can be made based on car make, year, model, vehicle class, transmission, and fuel type. A model can be developed to predict fuel consumption based on car features.  

The Data:
A dataset has been obtained from Government of Canada, published by Natural Resources Canada, for fuel consumption ratings. The dataset covers the period from 1995 - 2023 from original ratings for vehicles in Canada. This is the entire data that is available from the Government of Canada. The data was distributed across multiple csv files covering the different time periods, but files have been merged to reflect the entire timeframe from 1995 to 2023. The data source can be found in the "MY1995-2023 Fuel Consumption Ratings 5-cycle.csv" file.


Data Dictionary:
The dataset has the following 15 columns:

YEAR: The year the car model was made. It ranges from 1995 - 2023.
MAKE: The brand of the car.
MODEL: The corresponding model from the brand of the car. Some abbreviations:
            4WD/4X4 = Four-wheel drive
            AWD = All-wheel drive
            FFV = Flexible-fuel vehicle
            SWB = Short wheelbase
            LWB = Long wheelbase
            EWB = Extended wheelbase
VEHICLE: The class of the vehicle. 
TRANSMISSION: 
            A = Automatic
            AM = Automated manual
            AS = Automatic with select shift
            AV = Continuously variable
            M = Manual
            3 - 10 = Number of gears
FUEL TYPE:
            X = Regular gasoline
            Z = Premium gasoline
            D = Diesel
            E = Ethanol (E85)
            N = Natural gas
FUEL CONSUMPTION CITY (L/100 km): City driving conditions. Measured as litres of fuel per 100 km of driving.
FUEL CONSUMPTION HWY (L/100 km): Highway driving conditions. Measured as litres of fuel per 100 km of driving.
FUEL CONSUMPTION COMB (L/100 km): Combined city (55%) and highway (45%) driving conditions. Measured as litres of fuel per 100 km of driving.
FUEL CONSUMPTION COMB (mpg): Same as FUEL CONSUMPTION COMB (L/100 km) but in miles per gallon.
CO2 EMISSIONS (g/km): The tailpipe emissions of carbon dioxide (in grams per kilometre) for combined city and highway driving. 
CO2 RATING: The tailpipe emissions of carbon dioxide rated on a scale from 1 (worst) to 10 (best)
Smog RATING: The tailpipe emissions of smog-forming pollutants rated on a scale from 1 (worst) to 10 (best)
