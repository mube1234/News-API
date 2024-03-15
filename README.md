# Webz.io Free News API Lite Guide
Webz.io created the free [News API](https://webz.io/products/news-api#lite) Lite so students, developers, and researchers could easily incorporate high-quality, relevant news information into their non-commercial projects. The API gives you limited access to Webz.io vast repository of global news content, including up to 30 days of historical news data. It also includes advanced search capabilities so you can quickly refine and target your news data searches. With access to relevant and timely news data, you can discover trends and analyze sentiment. You can build innovative applications and dashboards powered by news data.
## Getting Started in 3 easy steps
You only need to complete three steps to use the News API Lite.
### 1. Request an API Key
* Go to the [News API web page](https://webz.io/products/news-api#lite).
* Enter your email to receive your API key.
  
![IMAGE1](https://camo.githubusercontent.com/f15e52caebf4961b7a568adf97013be43415e955197048aa22b96d342dc081f4/68747470733a2f2f7765627a2e696f2f77702d636f6e74656e742f75706c6f6164732f323032342f30332f46697273742d626f782e706e67)
### 2. Make an API Request
Use the API key provided to make your first call to the API. Make sure you also specify a search term in the request. For example, the following API request will return news articles related to the search term “Bitcoin.” The default time frame is 3 days, but you can set this to up to 30 days.
* `https://api.webz.io/newsApiLite?token=[token]&q=Bitcoin`

Here is a screenshot showing a part of the API call results in a web browser:

![IMAGE2](https://camo.githubusercontent.com/ec20debd2d15b23d43eabb867e4c5e19c55d6991d2784e9e0bf2b778ced52ba7/68747470733a2f2f7765627a2e696f2f77702d636f6e74656e742f75706c6f6164732f323032342f30332f737465702d322d4150492d63616c6c2e706e67)
### 3. Explore Webz.io news data
Experiment with different API call configurations, refining your searches with advanced features like [filters and Boolean queries](https://docs.webz.io/reference/news-blogs-discussions-api-overview). For example, you could search for news articles about U.S. President Joe Biden or his presidential challenger Donald Trump, refining the search to return articles with negative sentiment:

`https://api.webz.io/newsApiLite?token=[token]&ts=0&q=title%3A(Trump%20OR%20Biden)%20sentiment%3Anegative`

This query includes negative news posts about President Biden or Donald Trump in the past 30 days. Here is a screenshot of the call results in a web browser:

![IMAGE3](https://camo.githubusercontent.com/d3b6a5f96d880b3b38725c009e58adfc8dbbfe7d4813e2758f6856bcc458aca6/68747470733a2f2f7765627a2e696f2f77702d636f6e74656e742f75706c6f6164732f323032342f30332f737465702d332d636f727265637465642e706e67)
## Limitations
* Up to 1,000 calls per month.
* Returns 10 articles per call.
