# Stock-Status-Prediction-using-Tweet-Sentiment-Information

The python code to perform stock status prediction using twitter data sentiment information. This python code has six stages of data processing as shown in the figure below. 

![alt text](https://github.com/siddhaling/Stock-Status-Prediction-using-Tweet-Sentiment-Information/blob/master/fig.jpg)

### Stage 1: twitterDataDownload_1.py. 

This program downloads the tweets for the companies between the specified dates. The list company abbreviations are given in the file companyAbbvs.txt in the folder companyAbbvs. The tweets downloaded are stored in tweetsForAllCompany.JSON in the folder twitterData
### Stage 2: sentiAnalysisOfTweets_2.py.

This program performs the sentiment analysis of the tweets. The python code reads the tweetsForAllCompany.JSON file and computes the sentiments of tweets. The sentiment computed for the tweets are written as a file tweetsSentiScoreAndCls.csv in folder twitterData.
### Stage 3: collectFinanceDataYahoo_3.py.

This program fetches the finance data for a given list of company abbreviations from yahoo finance. The output is stored as stockPriceOpenAllCompany.JSON and stockPriceCloseAllCompany.JSON files in the folder yahooFinData.
### Stage 4: tweeterAndFianceFeaturesCombine_4.py.

This program combines sentiment information collected from tweets and finance data. It prepares a file stockpredict.txt and stored in the folder twFeaturesAndCls.
### Stage 5: predictStockStatus_5.py.

This program performs the prediction of stock status. The data set is read from the file stockpredict.txt of folder twFeaturesAndCls. The SVM classifier is created and on the data set, the cross-validation is performed. 

# Research Paper

This model of stock status prediction using tweet sentiment information has appeared in a research paper:

https://ieeexplore.ieee.org/document/8079788

https://www.youtube.com/watch?v=9AMdG_bnGFY

# Cite this work

Please cite as 

Siddhaling Urolagin, "Text Mining of Tweet for Sentiment Classification and Association with Stock Prices", IEEE International Conference on Computer and Applications (ICCA), pp 384-388, Dubai, 2017.

# Further Projects and Contact

For further reading and other projects please visit

www.researchreader.com

siddesh_u@yahoo.com


