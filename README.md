Twitter-scraping-with-snscrape-and-streamlit
APPLICATION LINK: https://tulasinnd-twitter-scraping-with-snscrape-twitter-scraper-sm39k5.streamlit.app/

Interative GUI using streamlit for twitter scraping

REQUIRED SKILLS:

Python scripting
MongoDB
Streamlit
Snscrape
OVERVIEW:

I have Created a GUI using streamlit that contains the follwing features

Can enter any keyword or Hashtag to be searched,
select the starting date
select the ending date
Number of tweets needs to be scrapped.
After scraping is done, it has the following options

Download data as CSV
Download data as JSON
Upload data to DATABASE
Display All the Tweets scraped
All the Uploaded Collections in Database are Displayed in the left side
WORKING:

Step1: Initially I collected the Keyword, Start date, End date, and Number of tweets from the user using streamlit

Step 2: The above details are fed to TwitterSearchScraper and TwitterHashtagScraper. A dataframe is created to store the entire scraped data Now we can download this scraped data in the form of CSV or JSON format

Step3: The database connection is established using pymongo A new collection will be created and data is uploaded into that collection if the user wish to upload

Step4: A separate sidebar is created to display all the collections that are uploaded to the database, On clicking any collection, we can see the documents in that collection

HOW TO RUN TWITTER SCRAPER IN YOUR MACHINE: open cmd:

C:\Users\mypc> pip install virtualenv

C:\Users\mypc> virtualenv my_twitter_env

C:\Users\mypc> cd my_twitter_env

C:\Users\mypc\my_twitter_env> cd Scripts

C:\Users\mypc\my_twitter_env\Scripts>activate # It will activate the virtual environment

(my_twitter_env) C:\Users\mypc> mkdir TwitterScraper #create a folder

(my_twitter_env) C:\Users\mypc> cd TwitterScraper # download the above files from this repository and place inside this folder

(my_twitter_env) C:\Users\mypc\TwitterScraper> pip install -r requirements.txt # it will install all the required modules in the environment

(my_twitter_env) C:\Users\mypc\TwitterScraper> streamlit run my_twitter_scraper.py # Now run the app using streamlit

You can now view your Streamlit app in your browser.

Local URL: http://localhost:8501
Network URL: http://192.168.107.230:8501
After clicking on the above url you can see the app in your browser
