# Sentiment-Analysis_Data Extraction_nlp

## Objective
The objective of this project is to extract textual data articles from the given URL and perform text analysis to compute variables as explained below.


## Data Extraction
For each of the articles given in the `input.xlsx` file, the article text is extracted and saved in a text file with URL_ID as its filename. The program extracts only the article title and the article text, excluding the website header, footer, or any other irrelevant information applying webscrapping using Newspaper library.

## Data Analysis
For each of the extracted texts from the articles, after cleaning the data and tokenizing it, textual analysis is performed to compute variables.
## Variables
The variables computed during the text analysis are as follows:

1. POSITIVE SCORE: The total score obtained by counting positive words in the text.
2. NEGATIVE SCORE: The total score obtained by counting negative words in the text.
3. POLARITY SCORE: The overall polarity (positive or negative) of the text, calculated as (Positive Score - Negative Score) / (Positive Score + Negative Score + 0.000001).
4. SUBJECTIVITY SCORE: The subjectivity of the text, calculated as (Positive Score + Negative Score) / (Total Words after cleaning + 0.000001).
5. AVG SENTENCE LENGTH: The average number of words per sentence in the text.
6. PERCENTAGE OF COMPLEX WORDS: The percentage of words in the text that are considered complex.
7. FOG INDEX: A measure of the readability of the text, calculated as 0.4 * (Average Sentence Length + Percentage of Complex Words).
8. AVG NUMBER OF WORDS PER SENTENCE: The average number of words per sentence in the text.
9. COMPLEX WORD COUNT: The total count of complex words in the text.
10. WORD COUNT: The total count of words in the text.
11. SYLLABLE PER WORD: The average number of syllables per word in the text.
12. PERSONAL PRONOUNS: The count of personal pronouns (e.g., I, we, my, ours) in the text.
13. AVG WORD LENGTH: The average number of characters per word in the text.

## Output Data Structure
The output data structure follows the format specified in the "Output Data Structure.xlsx" file. It includes all input variables from "Input.xlsx" and the computed variables from the text analysis.

## Text Analysis
The text analysis methodology implemented in this project includes the following aspects:

1. Sentimental Analysis: Determines the sentiment (positive, negative, or neutral) of the text.
2. Analysis of Readability: Calculates the readability metrics such as average sentence length and percentage of complex words.
3. Average Number of Words Per Sentence: Computes the average number of words in each sentence.
4. Complex Word Count: Counts the number of complex words in the text.
5. Word Count: Determines the total count of words in the text.
6. Syllable Count Per Word: Calculates the average number of syllables per word.
7. Personal Pronouns: Counts the occurrence of personal pronouns in the text.
8. Average Word Length: Computes the average number of characters per word.

After performing the analysis and calculating the variables all output were exported to excel file.
