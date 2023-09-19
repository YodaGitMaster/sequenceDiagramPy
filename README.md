# sequenceDiagramPy
Small python package to create sequence diagram of a program syntax for the website https://sequencediagram.org/

## Setup:
- make sure the functions have docstrings, argument type, return type and ```if __name__ == "__main__"```
- change the entry point to the python file
- copy the syntax to https://sequencediagram.org/

## example syntax
```
scrape_and_insert_titles->load_webpage_with_random_user_agent: URL (str)
scrape_and_insert_titles<--load_webpage_with_random_user_agent: webdriver.Chrome
note over load_webpage_with_random_user_agent:Loads a webpage with a random user-agent using Selenium.
scrape_and_insert_titles->BeautifulSoup: 
open_links->load_webpage_with_random_user_agent: URL (str)
open_links<--load_webpage_with_random_user_agent: webdriver.Chrome
note over load_webpage_with_random_user_agent:Loads a webpage with a random user-agent using Selenium.
```
