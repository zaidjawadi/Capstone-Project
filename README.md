README

## Fuel consumption of different car models in Canada ##


## Project Overview:


The Problem Area:
This project aims to explore the relationships between car features and CO2 emissions across car models in Canada. The goal is to be able to identify how much CO2 (in grams per km traveled) a car generates based on its features.  

The User:
Anyone interested in identifying how much CO2 a car with certain feature emits. This could be indiviual car owners or anyone interested in estimating how much of emitted CO2 are cars responsbile for. Given certain car features, and if annual milage traveled is known, one can calculate how much CO2 a car generates. If we know how many cars are in a given jurisdiction and the average annual milage of those cars, we can calculate the amount of CO2 emitted (in tonnes) annually by cars. 

The Big Idea:
Using readily available features of a car, the goal is to build a model that takes these features and accurately calculates how much CO2 (g/km) is generated.

The Impact:
CO2 emissions are responsible for global warming and climate change. By knowing how much CO2 is generated from vehicles, we can have a good estimate of the amount of CO2 cars are responsible for. With the growing demand for electric vehicles, one can see how CO2 levels from cars change over time as electric vehicles take a bigger share of the cars on the roads. 

The Data:
A dataset has been obtained from Government of Canada, published by Natural Resources Canada, for fuel consumption ratings. The dataset covers the period from 1995 - 2023 from original ratings for vehicles in Canada. This is the entire data that is available from the Government of Canada. The data was distributed across multiple csv files covering the different time periods, but files have been merged to reflect the entire timeframe from 1995 to 2023. The data source can be found in the "MY1995-2023 Fuel Consumption Ratings 5-cycle.csv" file.


Data Dictionary:
The dataset has the following 15 columns:

- YEAR: The year the car model was made. It ranges from 1995 - 2023
- MAKE: The brand of the car.
- MODEL: The corresponding model from the brand of the car. Some abbreviations:
     - 4WD/4X4 = Four-wheel drive
     - AWD = All-wheel drive
     - FFV = Flexible-fuel vehicle
     - SWB = Short wheelbase
     - LWB = Long wheelbase
     - EWB = Extended wheelbase
- VEHICLE: The class of the vehicle 
- CYLINDERS: Generally, the more cylinders an engine has, the more power is generated.
- ENGINE SIZE (L): The volume of fuel and air that can be pushed through a car's cylinders
- TRANSMISSION: 
     - A = Automatic
     - AM = Automated manual
     - AS = Automatic with select shift
     - AV = Continuously variable
     - M = Manual
     - 3 - 10 = Number of gears
- FUEL TYPE:
     - X = Regular gasoline
     - Z = Premium gasoline
     - D = Diesel
     - E = Ethanol (E85)
     - N = Natural gas
- FUEL CONSUMPTION CITY (L/100 km): City driving conditions. Measured as litres of fuel per 100 km of driving.
- FUEL CONSUMPTION HWY (L/100 km): Highway driving conditions. Measured as litres of fuel per 100 km of driving.
- FUEL CONSUMPTION COMB (L/100 km): Combined city (55%) and highway (45%) driving conditions. Measured as litres of fuel per 100 km of driving
- FUEL CONSUMPTION COMB (mpg): Same as FUEL CONSUMPTION COMB (L/100 km) but in miles per gallon.
- CO2 EMISSIONS (g/km): The tailpipe emissions of carbon dioxide (in grams per kilometre) for combined city and highway driving. 
- CO2 RATING: The tailpipe emissions of carbon dioxide rated on a scale from 1 (worst) to 10 (best)
- Smog RATING: The tailpipe emissions of smog-forming pollutants rated on a scale from 1 (worst) to 10 (best)


The features that were used for modeling are:
     - FUEL CONSUMPTION COMB (L/100 km)
     - ENGINE SIZE (L)
     - CYLINDERS
     - FUEL TYPE (X, Z, D, E)

The models developed were:
     - Linear regression
     - Ridge regression
     - Lasso regression
     - kNN
     - SVR
     - Random forest

All models performed well, with low MSE and high R-squared score close to 1. This is attributed to the high linearity between the features (particularly fuel consumption combined) and CO2 emissions. 
To calculate how much CO2 a car generates per km traveled, one can use the four aforementioned features, which are readily available, for a given car to calculate the amount of CO2 emitted. 
