# FordGoBike Trip Data
**by Abdelrahman Ragab**

**Dataset**

> The dataset used for this exploratory analysis consists of monthly individual trip rides data 2017

Data wrangling process:
fix multiple fields that are not in the correct dtype, i.e. start_time, end_time should be datetime type, user_type and member_gender should be categorical data type, etc
add new columns for trip duration in minute, trip start date in yyyy-mm-dd format, trip start hour of the day, day of week and month

filter out outlier ages from visual examination of the member age distribution and statistical percentile

cast 'start_dayofweek' to category dtype

cast 'start_month' to category dtype for easy plotting


**Summary of Findings**

In the exploration, I found that there are two types of user:

Subscriber

Customer

The number of trips peaked around 8-9am and 17-18pm during a day,
there were more trips on work days (Mon-Fri) compared to weekends.
The riding trips tend to be shorter on Monday through Friday compared to weekends. 
 usage of the bike sharing system on normal work days, while more casual flexible use on weekends.


Also I found most ages are between 25 to 40 years old for subscriber users,
and the customer users are between 21 to 30 years old. The number of trips are growing up for 21-30 years old over time,


There are a lot more subscriber usage than customers overall. 
The riding habit/pattern varies a lot between subscribers and customers.
Subscribers use the bike sharing system for work commnute thus most trips were on work days (Mon-Fri) and especially during rush hours (when going to work in the morning and getting off work in the afternoon),
whereas customers tend to ride for fun in the afternoon or early evenings over weekends. Subscriber usage peaks out on typical rush hours when people go to work in the morning and getting off work in the afternoon, which strengthened their usage purpose and goal of riding. 
Similar pattern was not observed among customers who tend to ride most in the afternoon or early evening for a different purpose than the subscribers.


**Key Insights for Presentation**

For the presentation, I focus on just the user types, gender, and age. I start by showing the percentage of bike rides for all user types subcriber and customer, it's show the subcriber users are 84.2% and that mean the customer users are 15.8%.
Then I plot the number of bike rides (trips) for each day based on gender that mean it's plot the number of trips for evryday to show trips number for each gender on all days.
In the end I show the number of bike rides over time based on age category. I divided members age into 5 categories in cleaning section:

Age between 11 to 20
Age between 21 to 30
Age between 31 to 40
Age between 41 to 50
Age between 51 to 60
Age between 61 to 70
Age between 71 to 80


Different usage pattern/habit between the two type of riders are seen from the exploration. 
Subscribers use the system heavily on work days i.e. Monday through Friday whereas customers ride a lot on weekends,
especially in the afternoon. 
Many trips concentrated around 8-9am and 17-18pm on work days for subscribers, 
yet customers tend to use more in the late afternoon around 17pm Monday to Friday.
The efficient/short period of usage for subscribers corresponds to their high concentration on rush hours Monday through Friday, 
indicating the use is primarily for work commute. 
The more relaxing and flexible pattern of customer use shows that they're taking advantage of the bike sharing system quite differently from the subscribers, heavily over weekends and in the afternoon, for city tour or leisure purpose probably.




