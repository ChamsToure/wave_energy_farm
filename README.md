# General information 

Wave energy is a rapidly advancing and promising renewable energy source that holds great potential for addressing the challenges of global warming and climate change. However, optimizing energy output in large wave farms presents a complex problem due to the expensive calculations required to account for hydrodynamic interactions between wave energy converters (WECs). Developing a fast and accurate surrogate model is crucial to overcome these challenges. In light of this, we have compiled an extensive WEC dataset that includes 54,000 and 9,600 configurations involving 49 and 100 WECs, coordination, power, q-factor, and total farm power output. The dataset was derived from a study published at the GECCO conference and received the prestigious Best Paper award. We want to acknowledge the support of the University of Adelaide Phoenix HPC service in conducting this research. For more details, please refer to the following link: https://dl.acm.org/doi/abs/10.1145/3377930.3390235.

## Features
The dataset includes 4 CSV files for 49 and 100 wave energy converters based on Perth and Sydney wave scenarios. The main goal is predicting the total power output of the wave farm based on the coordination of WECs (X1, Y1, X2, Y2,..., Xn, Yn). As the second plan, predicting the power output of each converter in the wave farm can be interesting. 

* X and Y - coordinates
* Power - individual power
* total power - total power of all the WECs
* qW - q-factor 

## Findings
There are many duplicates in the dataset (4540).

## Goal
* Predicting the total power output of the wave farm based on the coordination of WECs
* Predicting the power ouput of each converter in the wave farm

## Candidates for inaccuracy
* To small dataset -> need more data
* Not the right regression model -> Test many different regression models and measure their accuracy

## Potential Problems
* Cannot inference based on geodata from only 4 locations, especially with a relatively small dataset. 
* In what timeframe was the data collected? Becuase you cannot predict the total power over the year if it is also dependent of the seasons
* Why are there so many duplicates? 

## Instances
Each instance represents the coordination of wave energy converters in a wave farm plus the total power output and individual power of each converter and q-factor. 

## Source
https://archive.ics.uci.edu/dataset/882/large-scale+wave+energy+farm
Neshat, Mehdi, Bradley Alexander, Nataliia Y. Sergiienko, and Markus Wagner. "Optimisation of large wave farms using a multi-strategy evolutionary framework." In Proceedings of the 2020 Genetic and Evolutionary Computation Conference, pp. 1150-1158. 2020.
Link to research: https://dl.acm.org/doi/abs/10.1145/3377930.3390235.