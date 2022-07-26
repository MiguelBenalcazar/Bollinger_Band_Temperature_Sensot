# Bollinger Band
this repository contains an easy way to apply the Bollinger Band which is broadly used in fintech [1] to a sensor information.

this method uses a sensor information from a temperature sensor in file TS_30-08-2017.csv.

There are two functions in the file.

dataPreparation(df, k=2, window=20) it is for performing the analisys over  a dataset where df is the dataframe, k=2 since it represent the 95% of the standard deviation,
and  window will represent the size of the sampling data to perform the analysis.

dataPreparation_Plot(df, k=2, window=20, samples = 300): it is for performing the analisys over  a dataset where df is the dataframe, k=2 since it represent the 95% of the standard deviation,
, window will represent the size of the sampling data to perform the analysis. Finally, samples refers to the number of data to plot.

The following are the equations to calculate the upper band and the lowwer band

lowerBB(lower Bollinger Band) = avg - (k * stddev),
upperBB(upper Bollinger Band) = avg + (k* stddev)

  where avg  represents the moving average from the selected window
        k represents the how much of the standard deviation we want to use  ![](https://github.com/MiguelBenalcazar/Bollinger_Band_Temperature_Sensot/blob/main/standardDeviationImg.jpg)
        stddev represents the standar deviation from the selected windows
  
## Results


### window = 5, samples = 50
![](https://github.com/MiguelBenalcazar/Bollinger_Band_Temperature_Sensot/blob/main/BoliingerBand_w5_s50.png)
### window = 10, samples = 150
![](https://github.com/MiguelBenalcazar/Bollinger_Band_Temperature_Sensot/blob/main/BollingerBand_w10_150samples.png)


## Support
[1] https://www.investopedia.com/terms/b/bollingerbands.asp
