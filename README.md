## **Important Disclaimer Regarding the Challenge**
This paragraph do not intent to be part of the "Written Analysis of Results" requested in the challenge. It is written to justify the difference between the results obtained by me and those shown as the expected results for the Challenge. 
From my perspective there is an error in the information being selected to calculate the annual return of the shares. As it is expressed on Module 2 the suggestion is to compare closing price of the first day of trading of a stock with the closing price of the last day of trading by using the following formula:

(endingprice - startingprice) -1

The formula is correct, but the starting price to be used should be the opening price of the first day of trading and not the closing one. By using the methodology suggested in the module there is one day of trading not being considered, which is the return of the first day of training. The code being presented has been done considering the **opening price of the first day of trading**.
The only change needed in the code is replacing the number 6 for a 3 in the column taken for the starting price. 
 
 
 
# **Refactoring of All Stock Analysis Macro**
## Overview
We have created a Macro-enabled excel file, that have the possibility of running a macro from a bottom which allows Steve to analyze the dataset of stocks for the year 2017 and 2018.
This worksheet has achieved successfully the requirement of Steve, nevertheless He has the need of increasing the dataset to perform a much wider analysis of stocks. For a bigger dataset the designed macro could not be as efficient in processing time as if we refactor the code. 
This readme file summarizes the findings of the refactoring process and the efficiency in processing time achieved with the new code in comparison with the previous one. 
In addition of the requested information we have added the opening price and closing price for each Stock in the selected year. 

## Results

#### **Summary of Stocks Performance**

While both year ends with a similar trading volume which is US$ 3.3B in 2017 vs US$3.1B in 2018. One year is dramatically different from the other. 2017 was what is called a "Bull" market where most of the stocks register an increase in the value, on the contrary 2018 was a clear "Bear" market when almost all the shares register a loss. 

#### **Stocks results 2017**

Year 2017 ends with 11 out of 12 shares registering profits with a maximum return of 202.3% obtained by DQ in just one year. The only share running on red on this year was TERP with a -7,93%.

The following chart summarize the performance of the market:

![Summary 2017](/Resources/Stocks_Summary_2017.PNG)

 
    

#### **Stocks results 2018**
Year 2018 ends with 10 out of 12 shares on the red with a maximum yearly return of 97.91% obtained by ENPH. The worst performance was achieved by DQ that losses 61.8% of its value on 2018 going back to a similar price per share that the one registered at the beggining of 2017.
    
The following chart summarize the performance of the market:

![Summary 2018](/Resources/Stocks_Summary_2018.PNG)

#### **Conclusions about the Stock Market during 2017-2018**
Considering only two years of analysis the shares with better performance were ENPH (+364%), SEDG (180%) and RUN (102%), being ENPH the only one achieving positive returns in both years. 
     

### Refactoring code process achievements

Refactoring performed on the "All Years Analysis" code was extremely positive in terms of time-efficiency to perform the same task. It is important to mention that I have considered only the time that the code request to perform the part of the code being refactored. I decided to exclude those part that are equal on both code to have a better sense of the time reduction caused by the refactoring process, process such us formatting and defining variables were out of the timer on purpose. 

#### **Results obtained with previous code**
     
The original code requires on average 0.56 seconds to perform the analysis requested as shown on the secreen captures shown below:

![Original 2017](/Resources/VBA_Original_2017.png) ![Original 2018](/Resources/VBA_Original_2018.png)

### **Results Obtained with the code refactored**
    
With the new code the process of the information requested take on average 0,048 seconds, as shown below:
    
![Refactored 2017](/Resources/VBA_Challenge1_2017.PNG) ![Refactored 2018](/Resources/VBA_Challenge_2018.png)
        
### **Conclusion**
    
The new code proves to be more efficient reducing the time of executing the analysis in 91.32% from the previous one. This means that the new codes runs more than 10 times faster than its previous version.
    
![Conclusion](/Resources/Summary_Chart_Final.PNG)
    
## SUMMARY

### Advantages of refactoring a code
The advantages of working on refactoring a code is mainly related to the increase in efficiency that we could obtain on the time consumed for processing certain information. In order to perform a refactoring on an existing code the original code should be clearly written with as many comments as possible that allows the person executing the refactoring to easily understand the flow of the code.

The only disadvantage is the time consumed by the person who is refactoring the code. It will be important to assess if the benefits in efficiency while compensate the investment done in order to refactor the code. This would heavily depend on how good and self-explanatory the original code is and how often and for how long the code refactored would be used.

### Pros and Cose considering this case
On this particular case the original code was clearly explained by several comments and it was easy to understand, therefore the refactoring process was not that long. The increase in efficiency was so high, reducing the processing time to less than 10% of the original, than it is clearly it was very positive to be performed.

