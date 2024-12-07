# lam_final
Parting is such sweet sorrow. Not just for this class. This repo counts various legislation across the country to see most commonly-used words when regulating fetal disposition.


# NOTE: ChatGPT was used to troubleshoot this code, reducing redundancies and finding times that operations were repeated and a list was wrongly appended into another list.

# Analysis of LegiScan data set — 2016 legislative session

This repository contains data, analytic code, and findings that support portions of the article, “When These Lawmakers Regulate Grieving Pregnancy Loss, They Focus on Abortion,” published December 6, 2024. Please read that article, which contains important context and details, before proceeding.


# Data

This analysis uses a text file, then analyzes the findings through a Google Sheet.
The text come from the following sources:
Legiscan web search
bills_land: legislative language copy-pasted into a single .txt
The final spreadsheets can be viewed here: https://docs.google.com/spreadsheets/d/1raBixsOS8pjBgG1I7J3fVewo69r_hy2eBE662Cmy2RM/edit?usp=sharing. It contains, among others, the following tabs relevant to the analysis:
word_list — the raw export from Python
pivot_raw — a pivot table to finalize a top-10 wordcount
final - the top-10 list, with words excluded like "section" and "code."


# Methodology

The notebook AnnaLeah-leg_disposition_count-deliverable.ipynb performs the following analyses:

Part 1: Load and tokenify language
Load programs and .txt file, tokenifying as you bring it into the NLP system

Part 2: Remove stopwords and lemmatize
Append text into a list, removing stop words and lemmatizing.

Part 3: Load list into dataframe, count values
Bring the list into a dataframe and count values to discover how often terms have used.


# Outputs

The notebooks output this spreadsheet which contains the wordcount for terms in the bills: leg_wordcount.csv. Also in the folder is AL_AUL_NLP, the wordcount manipulated to narrow the wordcount down to the top-ten results.


# Running the analysis yourself

You can run the analysis yourself. To do so, you'll need the following installed on your computer:
Python 3
SpaCy


# Licensing

All code in this repository is available under the MIT License. The data file in the output/ directory is available under the Creative Commons Attribution 4.0 International (CC BY 4.0) license. All files in the data/ directory are released into the public domain.


# Feedback / Questions?

Contact Anna Leah at dear@annaleah.com
