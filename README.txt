PROJECT MILESTONE 1
For my project, I am interpreting holiday data collected from HolidayAPI.com. 
So far, I have linked the API and inputted my API key, hence, I can now access the data. 
I will be comparing the data of the US, Mexico and Canada, as they are all on the North American continent. 
Then I will also compare the data of US to some European countries, to see who has more holidays in the month of February for example. 
The HolidayAPI has lots of parameters to use, such as month and day as well. 
With the free version of this database, I can only compare up to 10 countries at a time and can only access 2020 data , which is limiting, but I can work with it to draw some conclusions regardless.

I am having issues writing the data to a CSV file, and have reached out for help...I created the file no problem in the code, but I can not get the data I want (2020 US, MX, CA data) to pull into the list for some reason. For purposes of getting it done, I tried copying the output and pasted it into the write csv function, but I know that's not the right or pretty way to do it. It didn't work either. Not sure how to fix this...

PROJECT MILESTONE 2
12/5 - Was finally able to get the data to write to a csv. I had been trying to write the data to a csv before converting it to a dataframe, which obviously doesn't work. I used json.normalize to create the rows and columns needed, and then wrote it to a csv file.

12/9 - Milestone complete, see below:
- Central Tendency questions - I posed two questions regarding mode, and one question was reviewed with two different blocks of code to confirm accuracy. Considering this dataset was largely comprised of qualitative data, it was difficult to pose different Central Tendency questions.
    - The only quantitative data in this data set was the dates of each holiday and the numeric day of the week that the holiday fell on.
    - I did what I could in this section, but all questions utilized mode. I tried using .describe() but it returned strange data with percentiles that did not make sense, as it was utilizing the dates. 

- Three questions for your analysis to answer & how the code got you to these answers
    - Question #1 - What are the number of holidays in each country? (USA, Canada Mexico)(In 2020)
        #using value counts
        #plot with bar graph to represent data visually as well
    - Question #2 - How many holidays are observed on each day of the week in 2020? (Cumulative totals across Canada, MX & USA data)
        #df into 'weekday.observed.name' column and used value counts
    - Question #3 - How Many Public Holidays are in each country?
        #used groupby 
        #added chart for visual representation
        #was also interested in the actual names of the public holidays in each country, used groupby() again, with get_group() for Canada and MX, then with the sort values function to see "true" public holidays and names for each country

- Two questions answered using graphs
    - I added graphs to two of the questions to allow for visual representation of data

- One example using group by
    - Noted above

PROJECT MILESTONE 3
(10%) Exploratory data exploration with some visualization. 
(60%) Data cleaning and feature engineering. You need to 
1) show at least one example of using the apply() or map() function to some features. 
2) show how to use one-hot encoding to transform a categorical feature; 3) Building the training set and the test set. 
(30%) Use the K-nearest neighbors (or another classification model of your choice) to solve your classification problem. 
Show at least some tuning of the model parameters and discuss how the training accuracy changes. 