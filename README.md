# TrustLabsAssesment

I divided this assessment in various parts:

First is to use Common Crawler in order to extract various indexes and download files of a particular domain.
Second is to filter on URLs which contain relevant information
Third is to perform sentiment analysis on the content

The pseudo code followed is :
1)Stored indexes for 2020 data from https://index.commoncrawl.org 
1)Search domain – Using Common-crawl- API to search for URLs
2)Adding all URLs to a list
3)For each URL, downloading the page 
4)Checking if the page contains the words COVID, hydroxychloroquine and chloroquine using full HTML Archive copy from Common- crawl
5)If the page does contains these words, I will go ahead to check the sentiment of the page to see if its score. 
6)If the score is towards extreme negative then the URL is definitely not supporting the use of those above chemicals hence can be rejected
   If score is between neutral to positive then URL can be considered for promoting use
7)The required URLs are then stored in a list and returned

I did some research on this topic on the net and saw that hydroxychloroquine and chloroquine not recently but around April 2020, hence I will majorly search for index in March, April, May 2020. 

As studies for the trials of the chemicals were then performed and they were later proven to be ineffective and fatal after May 2020, most websites have rejected the use of these chemicals for COVID treatment. 

In order to adhere to the short deadline of the assessment, I have considered only urls which have been updated earlier to that. There have been urls which have promoted the use recently as well but very less in number.

In order to look for domains, I could not go for all domains available so I started with covering news articles specifically those which weren't very popular in order to spread this wrong news. If time permitted, I would go over all news channels stored in a list. But for the scope of this assessment I have considered few.

Apart from sentiment analysis, I also aim to pass a list of strong positive words to match like effective, cure, heal, remedy, good, treat, prevent, spread, shorten which can also suggest that the website is promoting the use of these agents.

The work done so far shows the number of subdomains within a domain which contains misinformation websites.

Pending work : 
1) make a compact function for the above work 
2)get domain names of multiple news websites  and expand the same to twitter and facebook as these are the websites which spread misinformation fastest
3)add more matching patterns which could make corelation stronger in order to classify the website 
