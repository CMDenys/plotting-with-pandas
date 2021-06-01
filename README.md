In this hypothetical study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of a fictional pharmaceutical company, Pymaceutical, drug of interest, Capomulin, versus other treatment regimens. Included are tables and figures needed for the technical report of the study, as well as a top-level summary of the study results.

The first step in the study was to merge the data from multiple data sets.

<p align="center">
  <img src="images/1_merged_dfs.png" width="550" />
</p>

Once the data sets were merged, the data was checked for any mouse ID with duplicate time points.  It was found that mouse ID g989 had multiple time points listed, so data associated with that mouse ID was removed.  A check for the mouse count before and after the merge was conducted to ensure the data had been removed.  

<p align="center">
  <img src="images/2_mouseCheck.png" width="450" />
</p>
<p align="center">
  <img src="images/4_dfMerge.png" width="500" /> 
</p>
<p align="center">
  <img src="images/3_mouseCheck2.png" width="500" /> 
</p>

Once the clean data frame was created, using the groupby method, a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen was produced.

<p float="left" align="center">
  <img src="images/5_groupbySummary.png" width="400" />
  <img src="images/6_groupbyPic.png" width="400" />
</p>


Matplotlib's pyplot was used to show the total number of measurements taken for each treatment regimen throughout the course of the study.

<p float="left" align="center">
  <img src="images/7_barPlot.png" width="400" />
</p>


A pie plot was generated Pandas's DataFrame.plot() that shows the distribution of female or male mice in the study.

<p float="left" align="center">
  <img src="images/8_pieChart.png" width="400" />
</p>


Next, the final tumor volume of each mouse across four of the most promising treatment regimens were analyzed.  These were: Capomulin, Ramicane, Infubinol, and Ceftamin.  To determine if there are any potential outliers across all four treatment regimens, the quartiles and IQR and quantitatively calculated.

<p float="left" align="center">
  <img src="images/9_treatmentForloop.png" width="575" />
  <img src="images/10_box.png" width="400" /> 
</p>



Using Matplotlib, generate a box and whisker plot of the final tumor volume for all four treatment regimens and highlight any potential outliers in the plot by changing their color and style.
Hint: All four box plots should be within the same figure. Use this Matplotlib documentation page for help with changing the style of the outliers.


Select a mouse that was treated with Capomulin and generate a line plot of tumor volume vs. time point for that mouse.


Generate a scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen.


Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. Plot the linear regression model on top of the previous scatter plot.


Look across all previously generated figures and tables and write at least three observations or inferences that can be made from the data. Include these observations at the top of notebook.
