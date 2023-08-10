# Solar plant Efficiency
## Colin Lovestad

###stakeholder is small city council  considering allocation of funds to  start an off grid subdivision , with the question of  "how much power can be generated to support the subdivision and its network of buildings  and how reliable on a month to month basis will the generation be to gauge the need(if any) for alternative power sources(grid power)

- Power production predictions to gauge duty cycle of plant components  to maintain peak efficiency.
- This data has been gathered at a solar power plant  in India over a 34 day period. The power generation dataset are gathered at the inverter level - each inverter has multiple lines of solar panels attached to it. 
  
## Data source: https://www.kaggle.com/datasets/anikannal/solar-power-generation-data

## Data Dictionary: ![image](https://github.com/clovestad/Solar-Plant-Efficiency/assets/103072823/f71499ea-4367-411c-b476-bf07713ae709)

## Data Cleaning
### Task
- Identify and delete unnecessary columns.
- Check duplicates and permit high cardiality columns(source_ID)
- Deleted null duplicate rows.
- perform Feature engineering on datetime column to split into  better data fit for modeling.
- Produced univariate visuals.
- identify any outliers.

  ## Exploratory Data Analysis
  - ![image](https://github.com/clovestad/Solar-Plant-Efficiency/assets/103072823/454f0b52-6171-4506-b12c-dc61b3484910)
  - the above plot relates a majority of the inverters maintaining and steady output of 7.25Kw on a montly total output with a few inverters indicating inefficiencies that COULD effect overall plant performance/generation and should be noted for maintnience or replacement.
 
  - ![image](https://github.com/clovestad/Solar-Plant-Efficiency/assets/103072823/60be384d-4cc3-4ca2-ab2a-2300d05f5bfa)


  - the above table relates that the peak production hours are undoubtably in the midle of the day, while the sun is at its highest point.


## Modeling

 ###regression tree
 
  ![image](https://github.com/clovestad/Solar-Plant-Efficiency/assets/103072823/3bded2e3-9bb2-4b6b-aa7b-2f7a38f60434)


  ###descision tree tuned with gridsearch

  ![image](https://github.com/clovestad/Solar-Plant-Efficiency/assets/103072823/8ca472ee-1d65-4d3f-827a-5e9336b883ab)



# Model Selection

- the model that will be selected is the descision tree turned with gridsearch(best parameters)
- while it reflects the highest R2 score the true target is to discover and predict the need for preventative maintnience to Minimize plant downtime and production dips.
  

  
  


  



  

  
