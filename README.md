# P6: Make Effective Data Visualization

By Jen-Feng Hsieh


## Summary
This project will use JavaScript library D3 and Dimple to visualize data of Titanic incident which happened on April 15, 1912, and aims to discover stories of survival information from the data.

There are 891 passengers in the dataset, and 342 people of them were survived. The female has higher survival rate than male, and the passengers who purchased upper class have the highest survival rate.


## Design
Before visualizing data, I go over the dataset. There are 11 variables which are Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, and Embarked. There are many missing data of variable Age. The variables Name, Ticket, and Cabin are not very helpful when doing visualization, so I decide to plot the bar chart for the variables Survived and Sex, shown in index1.html. It is very obvious to understand survival of female is higher than male from the chart. 

After getting Feedback 1 and 2 from my friends, I think it would be better to add a description to help the reader understand the number of passenger, female, and male in the dataset. Therefore,  the reader can easy to understand how much people survived in each category. I also add the other variable Pclass to the chart. The class means the passenger's economic status. People have the higher level of class pay higher average price on fare than the lower level. The chart is shown in index2.html.

The Feedback 3 lets me think about it may be not very clear and difficult to connect the relationship between the number of survival people and total people in each category because each category has the large difference of total people. For example, there are 216 people are upper class, 184 are middle class, and 491 are lower class. Hence, so I decide to calculate survival rate in each category and also use animation to see the difference of survival rate between male and female. From the chart in index_final.html, the survival rate of female is much higher than male, and the higher level of class has higher survival rate than the lower level. I am very surprised that upper-class female has 96.81% survival rate.

Last, I would like to address how I design charts. There are three important categorical variables Survived, Pclass, and Sex. When I created the first chart, I set Sex as the x-axis and Survived as the y-axis. It is very clear to get the information from visualization. However, the reader still cannot get the whole picture of the story because there is no information of how many passengers in the ship. Therefore, I wrote the description in the second chart to help the reader understand the survival information. Besides, I also added the variable Pclass to see any difference of survived people between their economic status. Nevertheless, it seems the second chart shows too much unorganized information, and it's difficult to let the reader get information when they first glance. Thus, I changed the y-axis to survival rate which is calculated by the average of survived people in each categorical group. I also removed the gender from chart to legend and did the visual encoding of animation, so the reader can compare the class for the first time, and then the gender for the second. The number of passengers is also added in the tooltip.

## Feedback
Feedback 1 
> The chart is good, and it clearly shows the difference of survived people between male and female. However, it doesn't tell how many people in the data and how many people of gender.

Feedback 2
> It is interesting that survived people of female is double larger than male. Do you visualize other variables? There are only two variables in the chart, and it seems you still can add more variables, so the reader can obtain more stories.

Feedback 3
> The plot shows the survived of females is higher than males, but it seems no difference between each class.  


## Resources
1. Udacity Discussion Forum website
2. Dimple js website
- http://dimplejs.org/examples_viewer.html?id=bars_vertical_grouped
- http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control
3. Kaggle website
- https://www.kaggle.com/c/titanic
