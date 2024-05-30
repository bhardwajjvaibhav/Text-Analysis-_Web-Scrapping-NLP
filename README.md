# Text-Analysis_Web-Scrapping-NLP
Objective
The primary objective of this project is to extract textual data from given URLs and perform comprehensive text analysis on the extracted articles. The analysis involves computing various linguistic and readability metrics as specified.
Data Extraction
Input
•	Input.xlsx: An Excel file containing a list of URLs from which articles need to be extracted.
Process
1.	Reading Input: Read the list of URLs from the Input.xlsx file.
2.	Web Scraping: For each URL, scrape the article text including the title while excluding any other content like headers, footers, advertisements, etc.
o	Tools: Use Python libraries such as BeautifulSoup, Selenium, or Scrapy.
3.	Saving Extracted Data: Save each extracted article as a text file named with the corresponding URL_ID.
Data Analysis
Extracted Text Files
•	The text files generated from the extraction process serve as the input for this phase.
Variables to Compute
Using the definitions provided in the “Text Analysis.docx” file, compute the following variables for each article:
1.	Positive Score: Measures the number of positive words in the text.
2.	Negative Score: Measures the number of negative words in the text.
3.	Polarity Score: Indicates the overall sentiment of the text (Positive or Negative).
4.	Subjectivity Score: Indicates the degree of personal opinion versus factual information.
5.	Average Sentence Length: Calculated as the total number of words divided by the number of sentences.
6.	Percentage of Complex Words: The ratio of complex words (words with three or more syllables) to the total word count.
7.	Fog Index: A readability test that estimates the years of formal education needed to understand the text on the first reading.
8.	Average Number of Words Per Sentence: Similar to average sentence length, reaffirming sentence complexity.
9.	Complex Word Count: The total count of complex words in the text.
10.	Word Count: The total number of words in the text.
11.	Syllable Per Word: Average number of syllables per word in the text.
12.	Personal Pronouns: Count of personal pronouns (e.g., I, we, you, he, she).
13.	Average Word Length: The average length of words in the text.
Output
•	Output Data Structure.xlsx: The results of the text analysis should be saved in this Excel file, maintaining the exact order and structure specified.
Implementation
Step-by-Step Workflow
1.	Initialization:
o	Import necessary Python libraries: pandas for handling Excel files, requests for making HTTP requests, BeautifulSoup for parsing HTML, and re for regular expressions.
2.	Data Extraction:
o	Read the URL list from Input.xlsx.
o	For each URL:
	Make an HTTP request to fetch the web page.
	Parse the HTML content to locate the article title and body.
	Clean the extracted text to remove any non-article content.
	Save the cleaned text into a file named with the URL_ID.
3.	Text Analysis:
o	Read each text file.
o	Compute the required text analysis variables:
	Tokenize the text to count words, sentences, and syllables.
	Identify and count positive and negative words using predefined dictionaries.
	Calculate readability scores like Fog Index.
	Use regular expressions to identify personal pronouns.
o	Compile the results into a structured format.
4.	Output Generation:
o	Save the computed variables into Output Data Structure.xlsx in the specified format.
Tools and Libraries
•	Pandas: For reading and writing Excel files.
•	Requests: For HTTP requests to fetch web pages.
•	BeautifulSoup: For parsing and extracting data from HTML.
•	NLTK/Spacy: For natural language processing tasks such as tokenization and POS tagging.
•	Regex: For pattern matching in text analysis.
This project aims to automate the process of extracting and analyzing web articles to provide valuable insights into their content and readability.
4o


