# Homework 2 
---------------------------------

Homework 2 demonstates the following key concepts:  

- Scales
- Axes
- Loading Data 

-----------
### Data Source:

My dataset for this is assignment is [rundata.csv](https://github.com/estridge2014/d3_spring_2024/blob/main/Homework_2/rundata.csv) . Rather than defining a dataframe manually in the code I loaded the data with the following code. 

```javascript
//Load running data and related variables
        d3.csv("rundata.csv").then(data => {
            console.log("data", data)
        //format data
        data.forEach(d => { 
            d.Day = d.Day;
            d.Miles = +d.Miles; 
        });

//This data contains the number of miles I ran each day last week.
//Day == Which weekday (string)
//Miles == Miles ran (numeric) 
```

-------
### Assignment

I've created a barchart to visualize my data. The X axis displays days of the week, while the Y axis displays the number of miles I ran on that particular day.

<img width="512" alt="Screenshot 2024-03-12 at 12 00 06 PM" src="https://github.com/estridge2014/d3_spring_2024/assets/84936545/0d975c82-e86d-462a-acdd-3c4ecaa87ff9">
