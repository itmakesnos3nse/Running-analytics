# Running-analytics
Exploratory data analysis of the big dataset of ultra-marathon running

## File Description
The dataset contains 7,461,226 records of ultra-marathon races from 1,641,168 unique athletes.

The following columns are included (with data types):

1. Year of event (int64)
2. Event dates (object)
3. Event name (object)
4. Event distance/length (object)
5. Number of finishers (int64)
6. Athlete's result (object)
7. Athlete's club (object)
8. Athlete's country (object)
9. Athlete's birth year (float64)
10. Athlete's gender (object)
11. Athlete's age category (object)
12. Athlete's average speed (object)
13. Athlete ID (int64)

The "Event name" column includes information about the country and location, which can be extracted into a new column, and similarly, seasonal information can be found in the "Event dates" column after "Year of event" (this can be extracted with some processing).

The "Event distance/length column" describes the type of race, covering the most popular distances and lengths of UM races, as well as some other special modalities (multi-day, etc.):

Distances: 50 km, 100 km, 50 miles, 100 miles  
Time: 6 hours, 12 hours, 24 hours, 48 hours, 72 hours, 6 days, 10 days  
Additionally, other columns contain information about age, gender, and speed (in km/h).

## What Has Been Done
1. Changed the format of some data for convenience
2. Removed unnecessary records and columns
3. Selected a sample with data on 50 km and 50-mile races held in the USA in 2020

### From the selected sample, the following questions were answered:
1. How many times more runners are there in the 50 km races than in the 50-mile races?
2. What proportion of the two types of races are men, and what proportion are women?
3. How is the average speed distributed in each type of race for men and women?
4. Which age groups perform better in the 50-mile races? (>= 20 races)
5. Which age groups perform worse in the 50-mile races? (>= 10 races)
6. In which season do athletes run the distance faster?

The link to the dataset is in the Jupyter Notebook
