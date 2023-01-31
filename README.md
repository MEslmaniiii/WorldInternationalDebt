# World International Debt

 # The World Bank's international debt data¶
It's not that we humans only take debts to manage our necessities. A country may also take debt to manage its economy. For example, infrastructure spending is one costly ingredient required for a country's citizens to lead comfortable lives. The World Bank is the organization that provides debt to countries.

In this notebook, we are going to analyze international debt data collected by The World Bank. The dataset contains information about the amount of debt (in USD) owed by developing countries across several categories. We are going to find the answers to questions like:

What is the total amount of debt that is owed by the countries listed in the dataset?
Which country owns the maximum amount of debt and what does that amount look like?
What is the average amount of debt owed by countries across different debt indicators?
![image](https://user-images.githubusercontent.com/105324794/215667946-cb88c3c5-3552-4e8b-92d1-32000490c749.jpeg)

The first line of code connects us to the international_debt database where the table international_debt is residing. Let's first SELECT all of the columns from the international_debt table. Also, we'll limit the output to the first ten rows to keep the output clean.
![Screen Shot 2023-01-31 at 7 52 02 AM](https://user-images.githubusercontent.com/105324794/215668754-cb9a9e69-12a3-4046-bb73-fa324f6f6179.png)
# 2. Finding the number of distinct countries
From the first ten rows, we can see the amount of debt owed by Afghanistan in the different debt indicators. But we do not know the number of different countries we have on the table. There are repetitions in the country names because a country is most likely to have debt in more than one debt indicator.

Without a count of unique countries, we will not be able to perform our statistical analyses holistically. In this section, we are going to extract the number of unique countries present in the table.
![Screen Shot 2023-01-31 at 8 03 13 AM](https://user-images.githubusercontent.com/105324794/215670247-ea71e746-6475-4650-b897-2707841311d8.png)

# 3. Finding out the distinct debt indicators
We can see there are a total of 124 countries present on the table. As we saw in the first section, there is a column called indicator_name that briefly specifies the purpose of taking the debt. Just beside that column, there is another column called indicator_code which symbolizes the category of these debts. Knowing about these various debt indicators will help us to understand the areas in which a country can possibly be indebted to.

![Screen Shot 2023-01-31 at 8 05 19 AM](https://user-images.githubusercontent.com/105324794/215670429-d3d58efd-39f7-41e8-9232-881de8fa68fe.png)

# 4. Totaling the amount of debt owed by the countries
As mentioned earlier, the financial debt of a particular country represents its economic state. But if we were to project this on an overall global scale, how will we approach it?

Let's switch gears from the debt indicators now and find out the total amount of debt (in USD) that is owed by the different countries. This will give us a sense of how the overall economy of the entire world is holding up.

![Screen Shot 2023-01-31 at 8 06 11 AM](https://user-images.githubusercontent.com/105324794/215670543-e18ae8cb-5c0a-46ab-a371-9f0874b9427b.png)

# 5. Country with the highest debt
"Human beings cannot comprehend very large or very small numbers. It would be useful for us to acknowledge that fact." - Daniel Kahneman. That is more than 3 million million USD, an amount which is really hard for us to fathom.

Now that we have the exact total of the amounts of debt owed by several countries, let's now find out the country that owns the highest amount of debt along with the amount. Note that this debt is the sum of different debts owed by a country across several categories. This will help to understand more about the country in terms of its socio-economic scenarios. We can also find out the category in which the country owns its highest debt. But we will leave that for now.


![Screen Shot 2023-01-31 at 8 06 46 AM](https://user-images.githubusercontent.com/105324794/215670639-119c16bc-8f18-4589-b4de-f705ac3c3574.png)

# 6. Average amount of debt across indicators
So, it was China. A more in-depth breakdown of China's debts can be found here.

We now have a brief overview of the dataset and a few of its summary statistics. We already have an idea of the different debt indicators in which the countries owe their debts. We can dig even further to find out on an average how much debt a country owes? This will give us a better sense of the distribution of the amount of debt across different indicators.


![Screen Shot 2023-01-31 at 8 07 16 AM](https://user-images.githubusercontent.com/105324794/215670686-13ad4ab1-bc8d-46c9-88e7-bc1c05fbeabc.png)

# 7. The highest amount of principal repayments
We can see that the indicator DT.AMT.DLXF.CD tops the chart of average debt. This category includes repayment of long term debts. Countries take on long-term debt to acquire immediate capital. More information about this category can be found here.

An interesting observation in the above finding is that there is a huge difference in the amounts of the indicators after the second one. This indicates that the first two indicators might be the most severe categories in which the countries owe their debts.

We can investigate this a bit more so as to find out which country owes the highest amount of debt in the category of long term debts (DT.AMT.DLXF.CD). Since not all the countries suffer from the same kind of economic disturbances, this finding will allow us to understand that particular country's economic condition a bit more specifically.

![Screen Shot 2023-01-31 at 8 08 30 AM](https://user-images.githubusercontent.com/105324794/215670826-934d0e3a-f350-44b8-99d1-307be9d2598c.png)

# 8. The most common debt indicator
China has the highest amount of debt in the long-term debt (DT.AMT.DLXF.CD) category. This is verified by The World Bank. It is often a good idea to verify our analyses like this since it validates that our investigations are correct.

We saw that long-term debt is the topmost category when it comes to the average amount of debt. But is it the most common indicator in which the countries owe their debt? Let's find that out.

![Screen Shot 2023-01-31 at 8 09 06 AM](https://user-images.githubusercontent.com/105324794/215670905-6e0bcefc-c386-4e8e-8d67-07a8b28af5dd.png)

# 9. Other viable debt issues and conclusion
There are a total of six debt indicators in which all the countries listed in our dataset have taken debt. The indicator DT.AMT.DLXF.CD is also there in the list. So, this gives us a clue that all these countries are suffering from a common economic issue. But that is not the end of the story, but just a part of the story.

Let's change tracks from debt_indicators now and focus on the amount of debt again. Let's find out the maximum amount of debt that each country has. With this, we will be in a position to identify the other plausible economic issues a country might be going through.

In this notebook, we took a look at debt owed by countries across the globe. We extracted a few summary statistics from the data and unraveled some interesting facts and figures. We also validated our findings to make sure the investigations are correct.

![Screen Shot 2023-01-31 at 8 10 34 AM](https://user-images.githubusercontent.com/105324794/215671045-dfbe355d-24b7-4aee-b4ea-21aaf85f3d60.png)
