# bike-sharing  
## Problem Statement
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 
They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

  - Which variables are significant in predicting the demand for shared bikes.
  - How well those variables describe the bike demands

## Result
### Comparision between Training and Testing dataset:
- Train dataset R^2 : 0.826
- Test dataset R^2 : 0.7908
- Train dataset Adjusted R^2 : 0.823
- Test dataset Adjusted R^2 : 0.7828
- Demand of bikes depend on temp, windspeed, yr, season_summer, season_winter, mnth_September, weathersit_Light_Snow , weathersit_Mist

As per our final Model, predictor variables that influences the bike booking are:
Temperature (temp): A coefficient value of ‘0.5527’ indicated that a unit increase in temp variable increases the bike demand ( cnt ) by 0.5527 units.

Year (yr) : A coefficient value of ‘0.2332’ indicated that a unit increase in yr variable increases the bike demand (cnt) by 0.2332 units.

windspeed : A coefficient value of ‘-0.1552’ indicated that a unit increase in windspeed variable decrease the bike demand (cnt) by -0.1552 units. As windspeed is negatively correlated. bike hire prefer less windy days.

season_summer : A coefficient value of ‘0.0894’ indicated that a unit increase in season_summer ( summer season) variable increases the bike demand (cnt) by 0.0894 units.

season_winter : A coefficient value of ‘0.1281’ indicated that a unit increase in season_winter ( winter season) variable increases the bike demand (cnt) by 0.1281 units.

mnth_September : A coefficient value of ‘0.0894’ indicated that a unit increase in mnth_September ( September Month) variable increases the bike demand (cnt) by 0.0894 units.

weathersit_Light_Snow : A coefficient value of ‘-0.2785’ indicated that a unit increase in weathersit_Light_Snow ( Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds ) variable decreases the bike demand (cnt) by -0.2785 units. People doesnt prefer snowy , rain etc days as it harder to drive the bike.

weathersit_Mist : A coefficient value of ‘-0.0767’ indicated that a unit increase in weathersit_Mist ( Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist) variable decreases the bike demand (cnt) by -0.0767 units. People doesnt prefer Misty , mist +cloudy etc days as it harder to drive the bike because of poor visibility.
