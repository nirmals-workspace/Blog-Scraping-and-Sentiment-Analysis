# Blog-Scraping-and-Sentiment-Analysis
The primary goal of this project is to develop a systematic process for retrieving textual data from a specified URL, which contains articles. Once this data is collected, the next step is to conduct thorough sentimental and textual analysis to extract valuable insights and information.

## Prerequisites
Before you begin, you will need to have a few tools and libraries installed on your machine:
  - Python 3.7 or higher.
  - Requests, Beautiful Soup
  - Sklearn and NLTK Stopwords Corpus.
  - NLTK.
  - Numpy, Pandas, Matplotlib, Seaborn and Wordcloud.

## Project Structure

The project can be divided into several key components:

1. **Data Retrieval and Scraping**
   - The first step involves retrieving data from URLs specified in an Excel file (`Input.xlsx`).
   - Libraries like Requests and Beautiful Soup are used for this purpose.
   - The extracted article text is saved in separate text files with the `URL_ID` as the file name in a folder named `scraped_blogs`.

2. **Data Preprocessing**
   - To prepare the data for analysis, stopwords are collected from docx files in `stop words` folder and from nltk and sklearn stopwords corpus. Positive and Negative words are collected from docx files in `Master Dictionary` folder.
   - The collected stopwords and word dictionaries are used to clean the text data and compute sentimental and textual scores.

3. **Text Analysis**
   - This section focuses on computing various text analysis variables as outlined in the `Text Analysis.docx` document including sentiment scores and textual scores with formulas as given in the docx file.
   - Variables such as positive score, negative score, polarity score, subjectivity score, and more are computed for each article.

4. **Output Generation**
   - The computed variables are structured according to the format provided in the `Output Data Structure.xlsx` file.
   - The results are saved in an output Excel file.

5. **Data Visualization and Insights**
   - Further analysis is performed on the collected data starting with summary statistics.
   - Visualizations such as histograms, correlation map and wordcloud are used to understand the distribution of sentiment and textual scores.
   - Insights are drawn based on these visualizations and analysis.

## Insights

The project provides several insights based on the analysis:

- Sentiment Analysis:
  - Positive scores tend to be normally distributed, indicating that most articles are moderately positive.
  - Negative scores are right-skewed, suggesting that a majority of articles have low negativity, but some articles are overly negative.
  - Polarity scores are balanced between positive and negative trends.
  - Subjectivity scores indicate that most articles are objective.

- Textual Analysis:
  - Complex word count and the percentage of complex words are moderately distributed.
  - The Fog index shows some outliers, possibly due to varying writing styles.
  - Average sentence length ranges from 10 to 40 words per sentence.
  - Word count varies, with most articles falling between 300 and 1000 words.
  - Personal pronoun usage varies, with a majority having 2-3 personal pronouns.
  - Average word length is generally between 6-7 characters.

- Correlation Analysis:
  - Relationships between different text analysis variables are explored through correlation analysis and insights are derived and noted in the notebook.

- Word Clouds:
  - Word clouds are generated for the top 10 positive and top 10 negative articles and insights are noted.
  - Another word cloud is generated based on article titles and insights are noted.

## Future Improvements

- Expand the word dictionaries for sentiment analysis to improve accuracy.
- Enhance the text preprocessing steps for better data cleaning.
- Explore more advanced text analysis techniques and machine learning models.

## Contact
If you have any questions, comments, or suggestions for the project, please feel free to contact me at [nirmal.works@outlook.com]
