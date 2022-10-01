# PTT-crawler
This is the Taiwaese BBS, aka PTT, studyabroad forum crawler practice using python.

PTT website version homepage: https://term.ptt.cc/

PTT studyabroad forum: https://www.ptt.cc/bbs/studyabroad/index.html

## Prerequisite

- Python 3.6, 3.7 or 3.8
- Jupyter (Anaconda recommended)
- BeautifulSoup

## Usage

- Find topics using related keywords and designed the personal information form for the forum
- Allow for **simultaneous input** of multiple key words and **stored the corresponding URLS in excel**
- Adeptly operated **nested loops, if-else statements and BeautifulSoup** to build a well-functioning Web Crawler

## Program Details
1. How to crawl multiple web pages in PTT?
   - First, we observed that the website's url ends with *./index**XXXX**.html*, where XXXX indicates a sequence of number. Morevoer, the ***XXXX*** part decreases iteratively when letting the brower go to the webpages with older articles. 
   - Consequently, we can scrape the data from the forum by modifiying and iterating the ***XXXX*** part in the url.

2. The structure of nested loops
   - Three nested loops were used in the program, the outer loop is for iterating through the webpages, the middle loop is for searching the titles in a webpage and the inner loop is for matching the mutliple keywords that user inputs with the title.
   
3. title, title.a and title.a.string
   - In order to extract the necessary part (title string) from the HTML code, we use title.a.string to get the string between <a> and </a>

4. How to filter the topics that match with keywords?
5. How to store the data we scrape into excel

## Motivation

## Reference
