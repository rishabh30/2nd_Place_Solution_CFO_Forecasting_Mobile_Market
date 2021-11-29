

#### Project Title

# CFO Forecasting - Mobile Market - Sandesh Brand 2 - Final Challenge (June 2020)


### Problem Statement
Generate time-series forecasts with the highest accuracy predictions possible for only the 4 financial variables.
The time-series forecasts for two of the 4 variables (Revenue and ARPU Equipment) must also include 2 exogenous variables.
Targets must be Robust so as to be stable over a 6 month window.

## Project structure
├── data\
│   ├── Iphone_Data.csv\
│   └── Mobile_Sandesh_Brand_2_Refinement_Challenge_dataset.csv\
├── main.ipynb\
├── images\
├── report.pdf\
├── submissions\
├── requirements.txt\
└── License

### Prerequisites

```bash
pip install -r requirements.txt
```

### Robustness Methodology

- If the figure below is viewed, each horizontal line represents one iteration. Blue points are training window and (grey+red) points are forecasting/ prediction window(h = prediction window =4). In this diagram, each iteration has 4 forecasts. 
- Once all the iterations are done, RMSE is calculated for all h=1,h=2,h=3 and h=4. (h=1 means calculate the RMSE for all the iterations, for the first forecasted point, for h=2 calculate the RMSE for all the iterations for the second forecasted point….. same is repeated till h=4). Later these RMSE to be plotted in a graph. For more details https://otexts.com/fpp2/accuracy.html can be visited.

![robustness_methodolgy](images/robustness_methodolgy.png)

##### Results/Plots of some variables :


![variable1](images/1.png)

![variable2](images/2.png)

![variable3](images/3.png)

![variable4](images/4.png)

### Summary
- AutoRegressive Models
- Exogeneous Variables (iPhone launch insight data)
- Robustness
- Time-Series
- MAPE (Mean Absolute Percentage Error)
- AutoCorrelation
- Stationary Models

iPhone launch insight data
![imageiphone](images/imageiphone.png)
