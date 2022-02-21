# Kickstarting with Excel

## Overview of Project

The target outcome of this analysis is to find an optimal launch date and monetary goal amount for a better rate of success when launching a theater campaign using Kickstarter. The dataset provided for this analysis uses a vast array of data from multiple Kickstarter campaign categories.

### Purpose

The analysis exhibits the data to show the best months to launch a successful campaign and the optimum range for the monetary goal amount. The data is broken down into two categories; theater outcomes vs launch dates, and plays outcomes vs goal amount.

## Analysis and Challenges

A challenge with this analysis is extrapolating the relevant data to only show theater category and plays subcategories. The purpose of the analysis is to indicate when is the best month to launch a theater campaign, and what is the optimum range on a monetary goal amount for a Kickstarter campaign. Based on the original dataset categories and subcategories were required to be refined to remove the irrelevant data. Aside from the irrelevant data, the way dates were presented in the dataset was difficult to deduce based on how it was formatted. This challenge was overcome by using [Epoch Converter](https://www.epochconverter.com/) which reconfigured the composition of the data into measurable data. From this point, the sorted data was transferred into pivot tables and charts to be visualized.

### Analysis of Outcomes Based on Launch Date

The data on the chart “Theater Outcomes Based on Launch Dates” presents a count of the successful, failed, and canceled theater campaigns category based on monthly launch date. The chart layout represents the value or the count of campaigns on the left vertical axis. On the bottom horizontal axis the months are represented, starting from January on the bottom left; ending with December on the bottom right. The blue plotted line on the chart is representative of the successful campaigns. The red plotted line on the chart is representative of failed campaigns. And, the yellow plotted line on the chart is representative of canceled campaigns. The average count of successful campaigns within the 12 months is about 70 campaigns. Another data point represented in this chart is that the number of successful campaigns is not evenly distributed. The number of successful campaigns peak in May, and there on after begin to down trend. The lowest count taking place in December. The count of failed campaigns within the 12 months followed a similar (but flattened) trend as the successful campaign. The average count of failed campaigns for the 12 months is about 41 campaigns. Both the failed campaign and successful campaign show a similar peak trend in May but, the failed campaigns experienced a second peak in October. The failed campaign peak of october is inconclusive because although it can be explained by the declining number of successful campaigns after the May peak, failed campaigns seem to be affected disproportionately. The average count of canceled campaigns is about 3 campaigns over 12 months. The canceled campaigns line chart represents the highest count in January. October stands out due to the fact that there were no canceled campaigns during October, while the count of successful campaigns is declining, and the number of failed campaigns are rising.

![Theater_Outcomes_vs_Launch.png](resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

The data presented on the chart “Outcomes Based on Goals” is a percentage of successful, failed, and canceled Plays campaigns subcategory based on the monetary range of the Goal amount. The chart layout represents the Percentage of successful, failed, and canceled campaigns on the left vertical axis. On the bottom horizontal axis, the chart is representing the monetary range of the goal amount. Starting on the bottom left from less than $1,000 to more than $50,000 on the far bottom right. The blue plotted line on the chart is representative of the percentage of successful campaigns based on goal amounts. The orange plotted line on the chart is representative of the percentage of failed campaigns based on goal amounts. The silver plotted line on the chart is representative of canceled campaigns based on goal amounts. There is a strong trend between successful and failed campaigns displayed by the chart “Outcomes Based on Goals”. The successful campaign trends are tied to failed campaigns; as the percentage of successful campaigns starts to drop the percentage of failed campaigns will increase. There were similar trends or some relation between successful and failed campaigns on the previous chart “Theater Outcomes Based on Launch Dates” but not so tightly correlated as in this chart. Another data point this chart suggests is that higher goal amounts have a lower percentage of success.  

![Outcomes_vs_Goals.png](resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

Formating the data to obtain results for the chart “Outcomes Based on Goals” was challenging due to the range of monetary goal amounts. Using the formula [=COUNTIFS] was a difficulty encountered with this type of data, VBA would have been a useful resource when sorting data with changing arguments on Excel. The solution was to create a new worksheet with references for the arguments criteria on [=COUNTSIFS] formula. Self-reference the formula with the “find and replace” option to simplify the data on the final Excel worksheet.

## Results

-What are two conclusions you can draw about the Outcomes based on Launch Date? 
- May to December isn’t optimal to launch a theater campaign on Kickstarter.
- January to April have better odds of success for a theater campaign launch.

-What can you conclude about the Outcomes based on Goals?
- The optimal range of a monetary goal amount for a successful theater campaigns is less than $1,000 to $5,000. 
- Success rate of the campaign is diminished with the increased range for a monetary goal amount. 

-What are some limitations of this dataset?
- The dataset for "outcomes vs goals" measured goal range amount but the country or currency is not specified in the data.
- ($) is used as a reference to moneraty value since currency in unknown in the data. 

-What are some other possible tables and/or graphs that we could create?
- A graph displaying the duration of campaigns; Outcome vs Duration.
- The dataset lacked information on campaign's social media presence. 
