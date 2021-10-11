# Give-Life-Predict-Blood-Donations
The notebook shows what happened in detail through this investigation however below is a quick run down.

First, we loaded the data and explored it by inspecting the given columns. Below is a breakdown of the column.
R (Recency - months since the last donation)
F (Frequency - total number of donations)
M (Monetary - total blood donated in c.c.)
T (Time - months since the first donation)
a binary variable representing whether he/she donated blood in March 2007 (1 stand for donating blood; 0 stands for not donating blood).

Secondly, we decided to change one of the last columns that shared how many times a volunteer donated to the name "Target" column.
Thirdly, after seeing how many people had/not donated we wanted to break the data down to split it into a train and test dataset. 
After splitting the data we used a TPOT which is a Python automated learning tool that optimizes machine learning pipelines using genetic programming. 
The tool was able to help us predict the percentage change of the next volunteer coming back to donate.  The percentage ended up being 7850% however we wanted to take it a step further and worked on checking the variance of the columns. Through looking at the variance we decided to log normalize  the training data and perform the logistic regression again making the prediction slightly better from 7850% to 0.7891%
