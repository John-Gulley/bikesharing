# CitiBike Data Analysis
This week's project is focused on the analysis of bike sharing data. Specifically, we are working on CitiBike NYC Data to see how this business model can be applied and implemented in Des Moines (Iowa). The study includes the analysis of data from August 2019 as the summer months tend to have more traffic.
Overview of the Analysis
To convince investors that the bike sharing program in Des Moines is a solid business, we need to make a bike trip analysis and present it in a compelling way. To do so, we use Tableau Public and data from the Citi Bike System Data page.
# Results
The first step in our analysis is to pre-process the original data so the information has the correct datatype. We use Pandas to change the datatype of the Trip duration column from an integer to a datetime datatype so we can get the time in hours and minutes. Once the datatype is changed, the file is exported to the visualizations in the next part of the analysis. The Jupyter Notebook file is created for the analysis and are shown below.
  1.	Trips by Customer Type
The first interesting information of our analysis is related to the kind of customer that uses the bike service program. We already know that the total rides in the month of August is 2,344,224. Now we want to explore the types of customers and what is the proportion of short-term customers to the annual subscribers:
![image](https://user-images.githubusercontent.com/102339838/178396356-dd2838a0-f4a4-4040-bb2f-72a38f31e8eb.png)

  Figure 1. Customer Type Pie-chart
Approximately the 81% of the rides in the month of August corresponds to subscribers. Most of the users of the program are people that need to go around NYC in a daily basis, possibly people that live or work in the City. Since Des Moines is a capital city with great places to live and work, there is a potential market that could use the bike service program.
  1.	August Peak hours:
We now want to know the peak usage hours so we can get a better idea of how many bikes we might need in Des Moines, as well as figure out during which parts of the day we will need the most bikes:
 ![image](https://user-images.githubusercontent.com/102339838/178396451-f7eed07f-846f-4f1d-b76f-e6f94b45713d.png)

  Figure 2. August Peak Hour bar-chart.
As it was expected, the peak hours of bicycle usage coincide with the typical rush hours, around 8am and 5pm. This is explained since most of the customers are annual subscribers, who probably work in the City.
  1.	Checkout times:
Another interesting information we can analyze is the length of time that bikes are checked out for all riders. Figure 3 shows how the trips last less than one hour. In fact, the peak of ride-lasting time is around 15 minutes.
 ![image](https://user-images.githubusercontent.com/102339838/178396503-30ffa612-a267-43ab-81da-cc4d7ebe16bd.png)

Figure 3. Checkout Times for Users line-chart.
As an extension of this analysis, it is interesting to see how this ride-lasting information could be breakdown by Gender.
  1.	Checkout times by Gender:
The length of time that bikes are checked out for each gender is shown below.
 ![image](https://user-images.githubusercontent.com/102339838/178396571-13aa4abd-5ed0-4b26-ab42-32365aaf292f.png)

Figure 4. Checkout Times by Gender line-chart.
As it can be seen in figure 4, most of the users are males.
  1.	Trips by Weekday:
Our analysis and plots have shown that most of the users of the bike sharing program are males probably working around NYC. We now want to see how the number of bike trips vary by weekday for each hour of the day. The heatmap shown below display this relationship:
 ![image](https://user-images.githubusercontent.com/102339838/178396612-657fd8f4-470d-4f97-bcb0-5c17e833c945.png)

Figure 5. Trips by Weekday Heatmap.
There are two different patterns: one for days of the week and other for the weekend days. As it was expected, the weekdays show peak hours around 8am and 5-6 pm. However, for Saturday and Sunday there are blocks of hours of about seven to eight hours each day that have a high volume of trips.
1.	Trips by Weekday by Gender:
In order to go deep in the analysis of the previous results, we break down the number of bike trips by gender for each hour of each day of the week. Below it is the corresponding heatmap:
 ![image](https://user-images.githubusercontent.com/102339838/178396658-a59133d0-efd2-483d-96dd-308b5e1baba3.png)

Figure 6. Trips by Gender Heatmap.
Female and male patterns in the heatmap follow the same trend shown in figures 4 and 5. Because most of the users are males, the heatmap for males show a pattern more defined.
1.	User Trips by Weekday by Gender:
Finally, we want to see how the number of bike trips are broken down by gender for each day of the week and by each User type. Figure 7 shows the corresponding heatmap.
 ![image](https://user-images.githubusercontent.com/102339838/178396728-65c03309-cf34-43b1-9506-faa70e2f917e.png)

Figure 7. Trips by Usertype and Gender Heatmap.
As it was expected Customer Usertypes do not show any peak hours of bike usage. On the contrary, for subscribers, and specifically for male-subscribers, there are more use of bikes for every day of the week with respect to the female and unknown subscribers.
The complete story showing each one of the plots shown in this analysis can be seen in CitiBike story.
Summary
Our analysis of the NYC Citibike Data shows how most of the users of the program are subscribers, which leads us to think that the citibike users are generally people that live or work in NYC (people that need to go from one place to another place in a daily basis). This pattern coincides with the behavior reflected in the other plots shown in this analysis. For example, the peak hours bar chart shows how the bike-usage peak is around the traffic rush hours (8-9 am and 5-6 pm) which at the same time coincides with the working starting and ending hours. Our analysis also shows that most of the users are male and that the average duration of the trips is around 15-20 minutes.
For further analysis, it would be interesting to see:
•	The locations around the city that have more bike-traffic. This would help us to find areas where more bike stations are needed and also to decide the number of bicycles needed in each station.
•	Another interesting plot could be the number of trips by age of the users, this can help to understand in more detail the type of customer that is interested in the bike-sharing program.
