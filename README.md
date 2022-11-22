
# hawker
A python service package to download Bangladeshi Newspaper articles periodically

## DAY-1 (22 November 2022)

When the code is run
1. A CRON job will be added that runs periodically to scrape News papers
2. All scraping should run paralelly. At least a thread pool should be used  
   to scrape more than one source at a time. 
3. A source's front page will be scraped for new content.
4. All new content will be added to the ArticleStorage(Database).

### Tools  
1. Scrapy -- To scrape the source.
2. SQLAlchemy -- To Access and use the Database(Postgresql)
3. RQ -- To queuing job and running jobs in background

### Goals
1. Deploy the service at AWS
2. Build an archive of news articles of Bangladesh
3. The service should be resilient of restarts and other incidents
4. A proxy service should be used to avoid bot detections
5. At least three Newspaper should be scraped at first phase