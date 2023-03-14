# Mars_Webscraping_Challenge
Scrape and Analyze Mars Weather Data 

## Extracted News Articles 
Created a Beautiful Soup object to extract text elements from https://static.bc-edx.com/data/web/mars_news/index.html.

Extracted titles and preview text of news articles and stored the scraping results in Python data structures:

Stored each title-and-preview pair in a Python dicitonary and gave each dictionary two keys: title and preview.

Stored all the dictionaries n a Python list.

Exported scraped data to a JSON file.
![article_list.json](https://github.com/SheTroxel/Mars_Webscraping_Challenge/blob/main/aricle_list.json)

## Extracted Weather Data
Created a Beautiful Soup object to scrape temperature data for Mars from the html table at https://static.bc-edx.com/data/web/mars_facts/temperature.html.

The scraped table data was assembled into a Pandas DataFrame using the heading names for column headings.

Data types were evaluated and convereted where appropriate to dateime, int, or float data types.

Data file was exported as csv file.

![mars_tem_data.csv](https://github.com/SheTroxel/Mars_Webscraping_Challenge/blob/main/mars_temp_data.csv)

## Analysis of Data
Analyzed the dataset by using Pandas functions to answer the following questions about Mars.

How many months exists on Mars? 
12

How many Sols (Martian Days) worth of data exist in the scraped dataset? 
1867

What are the coldest and warmest months on Mars (at the location of Curiosity)? 
Plotting the average low temperature on mars we can determine on average the coldest month is the 3rd month. On average the warmest month is the 8th month.

![avg_low-tempertuare on Mars](https://github.com/SheTroxel/Mars_Webscraping_Challenge/blob/main/avg_temp.png)

Which month, on average, has the lowest atmospheric pressure? The highest?
Plotting the average atmospheric pressure by month, we can determine that atmospheric pressure on average is lowest in the sixth month and highest in the ninth.

![avg_pressure on Mars](https://github.com/SheTroxel/Mars_Webscraping_Challenge/blob/main/avg_pressure.png)

How many terrestiral days exist in a Martian year using a visual estimate?
Plotting all temperatures gather by Sols (Martian Days), the distance from peak to peak is roughly 1425-750, or 675 days. A year on Mars appears to be about 675 days from the plot. An internet search confirms that a Mars year is equivalent to 687 earth days.

![Minimum Temp by Day (Celsius)](https://github.com/SheTroxel/Mars_Webscraping_Challenge/blob/main/daily_temps.png)

Website Source: https://mars.nasa.gov/resources/21392/mars-in-a-minute-how-long-is-a-year-on-mars/#:~:text=The%20Earth%20zips%20around%20the,year%20means%20longer%20seasons%20too.
