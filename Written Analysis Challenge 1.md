# Kickstarting with Excel

## Project Overview and Purpose
The Project required analyzing data about how launch date and fundraising goals impact on fundraising outcomes.  Visualizations were created to show what launch dates and goals were most and least successful.  The data allowed some conclusions to be drawn about the best time or year the launch a campaign and the optimal size.


## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In order to compare outcomes based on launch date a pivot table was created showing outcomes - successful, failed, or cancelled by month launched.  The data was further filtered to only show theater campaigns.  Selecting the launch date by month was somewhat trick and I had to look up how to do it.    

### Analysis of Outcomes Based on Goals 
Next we wanted to compare outcomes based on goals.  I created a new sheet groups outcomes - suscessful, failed, or cancelled based on ranges of the intitial goal set.  I used the countifs function to search the and count the data.  It did take me some time to build he countifs functions and check them.  Example formula below:

=COUNTIFS('New Name'!$D$522:$D$4115,"<1000",'New Name'!$G$522:$G$4115,"successful",'New Name'!$R$522:$R$4115,"plays")

Next using the results from the countifs function I calculated the % successful/failed/cancelled by initial goal.  Then built a line chart the help visualize the results.  The most difficult part of building the line chart was getting the formatting right on the X axis, the labels were very crowded.  

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Don't launch a fundraising campaign around the December holidays.  December had the worst ratio of successful vs failed campaigns of any month of the year.  The best time to launch a campaign appears to be the Summer months - specifically May, June, and July.  These months had the most successful campaigns and all had a higher % of success than the average for the year.

- What can you conclude about the Outcomes based on Goals?
Smaller campaigns have a greater liklihood of success.  With the exceptions of some outliers as goal size increased, % success declined.

- What are some limitations of this dataset?
The sample size on larger campaigns was small making it hard to draw conclusions on campaings with goals greater than 25k.
  
- What are some other possible tables and/or graphs that we could create?
Looking at the % success by month would have been interesting to visualize with a chart.  Looking at average donar size by campaign goal could also have been relevant.