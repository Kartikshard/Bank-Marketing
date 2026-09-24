numerical_columns=['age','balance','day','duration','campaign','pdays','previous']

age-
age spread is good , no negative age

balance-
data['balance'].describe()
count     4521.000000
mean      1422.657819
std       3009.638142
min      -3313.000000
25%         69.000000
50%        444.000000
75%       1480.000000
max      71188.000000
366 rows have negative and total 733 have balance less or equal to 0 why?

day-prob means data , nice spread 0-31 no issue in sight
duration-last call duration in seconds
count    4521.000000
mean      263.961292
std       259.856633
min         4.000000
25%       104.000000
50%       185.000000
75%       329.000000
max      3025.000000
prob effect outcome strongest 

camapign-no. of calls made to this client during this campaign skewed data to right
pdays- number of days theclient was contacted from prev campaign -1 menas client not contacted yet
 THERE ARE CLIENTS WHERE IS y who are still uncontacted , and all their poutcomes are unknown
previous - number of calls performed before this campaign , data is spread to uneven