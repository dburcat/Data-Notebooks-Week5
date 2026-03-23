### Prerequisite 

* [NOAA Daily Summaries](https://github.com/Zipcoder/DataEngineering.Labs.NOAADailySummaries/blob/master/README.md)
* [Pip Module](https://github.com/Zipcoder/PythonFundamentals.Labs.PipModule)


### Part 1

In the NOAA Daily summaries lab, we looked at min and max temperatures for a particular location during each day of December 2018. For this lab, we are going to take a broader approach.
Let's get some data for the Global Summary of the Month dataset (the id for this dataset is called GSOM).

Acquire at least 70 years of data for this dataset. You should limit the datatype to TAVG.

| parameter  | value      | 
| ---------- | ---------- |
| datasetid  | GSOM       |
| locationid | FIPS:10003 |
| startdate  | *          |
| enddate    | *          |
| limit      | 1000       | 
| offset     | 1          | 
| datatypeid | TAVG       | 

&ast; startdate - for the first request the startdate attribute should be 1938-01-01. The second request should be 1948-01-01 and so on.  
&ast; enddate - for the first request the enddate attribute should be 1947-12-31. The second request should be 1957-12-31 and so on.

Save these files to ./data/monthly_summaries.

You should end up with a list of files as similar to this:

* FIPS10003_avg_1938_to_1948.json
* FIPS10003_avg_1948_to_1958.json
* ...
* FIPS10003_avg_2008_to_2018.json

### Part 2

Now that we have some data, open and complete the notebook called "loading_and_graphing_monthly_summaries.ipynb".

