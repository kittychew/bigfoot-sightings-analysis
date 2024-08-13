# Bigfoot, Big Data

Contributors: Kat Chu, Quinn Daley, Mackenzie Deets, Oumar Diakite, Jacob Woolley

## Project Summary
Bigfoot sightings are bizarre but common stories found in tabloids and campfire stories across America, but where and when and how to these mysterious sightings occur?
We sought to use the techniques and methods taught to us in class to analyze data from the Bigfoot Field Reaserchers Organization (BFRO) to make some key analyses broken down by time, location, and weather.

We approached this collaborative effort by independently doing analysis on one or two broader questions each, and coming together at the end to combine our results.

## Project Analysis

### Kat


### Quinn
In this section, we wanted to understand the overall number of Bigfoot sightings by year, focusing on how the number of reports has evolved over the years in respect to  differences in sighting types to gain deeper insights into the nature and timing of these reports. The code reads in JSON and CSV data files using Pandas, then displays the first few rows to preview. From there, the data was cleaned  by dropping NaN values in the 'YEAR' column, converting the 'YEAR' to an integer, and filtering the data for valid years. The code then groups the data by 'YEAR' and 'REPORT_CLASS', counts the occurrences, and pivots the data for plotting. Finally, it plots the number of Bigfoot sightings by year and report class using ,atplotlib, saving the plot as a PNG file. The figure that was created by the code illustrates the trends in Bigfoot sightings over time, categorized by different types of reports, allowing us to explore how these sightings have changed and varied across different classes over the years.

### Mackenzie


### Oumar


### Jacob
I was tasked with making analyses on the weather conditions during sightings. I began by reducing the geocoded data to only relevent columns and cleaning the data of rows with missing values. Columns with excessive amounts of missing data were excised entirely as to keep the data set at a suitable size.

My first analysis would be on the condition of the weather (e.g rain, snow, overcast) on sightings as maybe more hazy weather would make people easier to confuse something innocuous for a sasquatch. I did this by first relabeling the many listed conditions down to five based on the most extreme condition listed. (Snow > Rain > Overcast) and putting these in a bar chart which revealed rain to be the most common weather and overcast without precipitation to be the least common.

Then I decided to do a linear regression on cloud cover versus visibility to see if weather was impacting peoples perception as much as I expected. After doing so and charting it, I found no significant relationship between the two. I then decided to seperate the data points on this scatter chart by classification, but this also showed no obvious pattern.

Finally, I decided to run T-tests on some key conditions between Class A and Class B to see if weather would impact people's confidence in their sightings. I found that only humidity, cloud cover, and barometric pressure showed any significant difference, and when comparing summary stats, found that Class A was  slightly higher across all three categories.

## Credits

Original data from BFRO.net

Initial data scrape and project inspiration by Timothy Renner: https://data.world/timothyrenner/bfro-sightings-data
