# CS-410-IMDB-Sentiment
CS 410 Project

Installation and Execution
1.	Install the following libraries – 
pip install scrapy
pip install beautifulsoup4
pip install sklearn
pip insall joblib
pip install pickle

2.	The model has already been trained using sample data - http://ai.stanford.edu/~amaas/data/sentiment/

3.	Use this model to give Positive/negative score

4.	To Scrape user review for any movie, update the link at line # 9 in “Imdb/Imdb/Spiders/imdb_spider.py” 
(In IMDB, each Movie/TV Show has a title, which is used in the URL. The title for TV Show Manifest is tt8421350, so the link should be https://m.www.imdb.com/title/tt8421350/reviews)

5.	Run “scrapy crawl imdb” while inside the “Imdb/” directory. This will crawl and store the reviews in the folder “Imdb/Imdb/Spiders/” with “.json” extension 

6.	Copy the file and paste it in the main folder where the file “read_score.py” exists

7.	Run “python read_score.py” this will predict the reviews in the json file and output the scores in “output_sentiment.csv” file

