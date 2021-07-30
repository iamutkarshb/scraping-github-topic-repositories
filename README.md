# Python Web Scraping Project
Scraping Top Repositories for GitHub Topics

![](https://i.imgur.com/6zM7JBq.png)

Web scraping is the process of extracting and parsing data from websites in an automated fashion using a computer program. It's a useful technique for creating datasets for research and learning. Follow these steps to build a web scraping project from scratch using Python and its ecosystem of libraries:

TODO (Intro):

Introduction about web scraping
Introduction about GitHub and the problem statement
Mention the tools you're using (Python, requests, Beautiful Soup, Pandas)
Here are the steps we'll follow:

We're going to scrape https://github.com/topics
We'll get a list of topics. For each topic, we'll get topic title, topic page URL and topic description
For each topic, we'll get the top 25 repositories in the topic from the topic page
For each repository, we'll grab the repo name, username, stars and repo URL
For each topic we'll create a CSV file in the following format:
Repo Name,Username,Stars,Repo URL
three.js,mrdoob,69700,https://github.com/mrdoob/three.js
libgdx,libgdx,18300,https://github.com/libgdx/libgdx
Scrape the list of topics from Github
Explain how you'll do it:

use requests to download the page
user Beautiful soup to parse and extract information
convert to Pandas Dataframe

1. **Introduction to our project**
    - We're going to scrape https://github.com/topics
    - We'll get a list of topics. For each topic, we'll get topic title, topic page URL and topic description
    - For each topic, we'll get the top 25 repositories in the topic from the topic page
    - For each repository, we'll grab the repo name, username, stars and repo URL
    - For each topic we'll create a CSV file in the following format:
    
    ```bash
     Repo Name,Username,Stars,Repo URL
     three.js,mrdoob,69700,https://github.com/mrdoob/three.js
     libgdx,libgdx,18300,https://github.com/libgdx/libgdx 
     ````

2. **Use the requests library to download web pages**

    - Inspect the website's HTML source and identify the right URLs to download.
    - Download and save web pages locally using the `requests` library.
    - Create a function to automate downloading for different topics/search queries.


3. **Use Beautiful Soup to parse and extract information**

    - Parse and explore the structure of downloaded web pages using Beautiful soup.
    - Use the right properties and methods to extract the required information.
    - Create functions to extract from the page into lists and dictionaries.
    - (Optional) Use a REST API to acquire additional information if required.


4. **Creating CSV file(s) with the extracted information**

    - Create functions for the end-to-end process of downloading, parsing, and saving CSVs.
    - Execute the function with different inputs to create a dataset of CSV files.
    - Verify the information in the CSV files by reading them back using [Pandas](https://pandas.pydata.org).

**Notes**
Refer to the Jupyter notebook, documentation added. 
The Final code comprise of all the code we have done above and also scrapping of the top 25 repositories out of a topic page.
