# financial_analysis

## Code Notes
* When cleaning data, I changed the names of the portfolios to shorter versions to make the later resulting tables and graphs look cleaner. 
* The S&P500 returns information imported as a string with a dollar sign, so I had to replace the $ with an empty space, then I was able to convert the string to an integer. 
* All plots are visualized without issues after this. 
* When importing my three stock csv files for my own portfolio, I was able to find the syntax to ask google finance to give me just the close information, so that way I did not have to drop extraneous columns during data cleaning.
* During importing the csv files, I dropped the date column in the 2nd and 3rd file. I knew I was able to do this because I had requested the exact same date ranges for all three csv files when using google finance. This way I did not have duplicate date columns in my concatenated dataframe later on. 
* I also changed the date column from a string to datetime format and then dropped the timestamp in order to have the data look clean when joined with the combined returns dataframe, which did not have a timestamp in the date index. 
* When I concatenated the combined returns with my portfolio returns, it gave me a warning regarding the timestamp, probably stemming from my changing the datetime format of my portfolio in order to get rid of the irrelevant timestamp. It was successful nonetheless, and this did not hinder my ability to concatenate and show my returns against the other portfolios. 

