# Virat_Kohli_Performance_Anaylisis_using_Python
# [Check out my colab file👈](https://colab.research.google.com/drive/1kZp52l6SArYRQsVQqd9-x3RVNO4z2XqF?usp=sharing)
 ## Abstract of the project:
 The project "Virat Kohli Performance Analysis using Python" aims to analyze the batting performance of the acclaimed Indian cricketer Virat Kohli in One Day Internationals (ODIs). Using Python and popular data analysis libraries, the project explores key aspects such as runs scored, balls faced, boundaries hit, strike rate, batting positions, dismissal types, opposition teams, and playing grounds. The methodology involves data cleaning, preprocessing, and visualization using Python libraries such as pandas, matplotlib, and Plotly. The project provides insightful visualizations and an in-depth analysis of Virat Kohli's performance, making it valuable for those interested in sports analytics and data science involving cricket statistics.
 
###Libraries Used in the project:
1.pandas: import pandas as pd
Used for data manipulation and analysis, including reading and cleaning the dataset.
2.numpy: import numpy as np
Provides support for large arrays and matrices, along with mathematical functions to operate on these arrays.
3.plotly.express: import plotly.express as px
Used for creating quick and easy visualizations, such as line charts and scatter plots, to display the trends and relationships in the data.
4.plotly.graph_objects: import plotly.graph_objects as go
Provides more control and customization options for creating advanced visualizations like pie charts.
###Functions and Methods used in the project:
1.pd.read_csv("Virat_Kohli.csv")
Reads the dataset from a CSV file into a DataFrame for analysis.
2.pd.DataFrame(data)
Converts the data into a DataFrame object for easier manipulation and analysis.
3.data.head()
Displays the first few rows of the dataset to get an initial understanding of the data structure.
4.data.isnull().sum()
Checks for any missing values in the dataset to ensure data completeness.
5.data["Runs"].sum()
Calculates the total runs scored by Virat Kohli over the specified period.
6.data["Runs"].mean()
Computes the average runs scored by Virat Kohli, providing insight into his performance consistency.
7.px.line(data, x=matches, y="Runs", title='Runs Scored by Virat Kohli Between 18-Aug-08 - 22-Jan-17')
Creates a line chart to visualize the trend of runs scored over time.
8.data["Pos"].map()
Maps numerical batting positions to their corresponding string labels for better readability in visualizations.
9.go.Figure(data=[go.Pie(labels=label, values=counts)])
Creates a pie chart to show the distribution of matches played at different batting positions.
10.data.query("Runs >= 100")
Filters the dataset to include only the matches where Virat Kohli scored a century, used for further specific analysis.
11.px.bar(data, x=data["Opposition"], y=data["Runs"], color=data["Runs"], title="Most Runs Against Teams")
Generates a bar chart to show the runs scored against different teams.
12.px.scatter(data_frame=data, x="Runs", y="4s", size="SR", trendline="ols", title="Relationship Between Runs Scored and Fours")
Creates a scatter plot with a trendline to explore the relationship between runs scored and the number of fours hit.
