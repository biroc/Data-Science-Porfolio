Global News Tone Analysis and Visulization
------------------------------------------

Analyze global news average tone from GDELT Global Knowledge Pubic Dataset in Big Query

100,000,000 global news with domain, tone, country mentioned in the news attributes.
Tones toward other countries is calculated based on the countries mentioned in the news and the normalized average new tone.

The analysis is doen in both Pandas and Spark environment

Background Information
----------------------

Tone:

This is the average “tone” of the document as a whole.The score ranges from -100 (extremely negative) to +100 (extremely positive). Common values range between -10 and +10, with 0 indicating neutral. This is calculated as Positive Score minus Negative Score.

Positive/Negative Score:

This is the percentage of all words in the article that were found to have a positive/negative emotional connotation. Ranges from 0 to +100.

Overall Tones:

Average Tones of Chinese News: 0.07135

Average Tones of U.S. News: -1.2975

Average tones of U.K. News: -0.776

Output Analysis Result
------------------------------------------

General Average tone in Chinese news toward rest of the world

General Average tone in U.S. news toward rest of the world

General Average tone in U.K. news toward rest of the world

Average tone in Chinese news in special theme toward rest of the world

Average tone in U.S. news in special theme toward rest of the world

Average tone in U.K. news in special theme toward rest of the world

Requirement
----------------------

### Install the requirements
 
* Install the requirements using `pip install -r requirements.txt`.
    * Make sure you use Python 2.7.
    * Make sure you use Spark 1.6
    * You may want to use a virtual environment for this.

Usage
-----------------------
* Downloan GDELT Global Knowledge from Bigquery
	* Save the GKN data as .csv format

* Run `mkdir Data` to create a directory for our GKN data.

* Run `cd Data`
	* Run `mkdir General` to store the General Tone Data
	* Run `mkdir Theme` to store the Theme Tone Data
	* Save Theme data and General data into Theme/General folder respectively

* Run  `main.ipynb` in jupyter notebook to analyze global news average tone in Pandas
	* This will create China/US/UK's global news tone

* Run `theme.ipynd` in jupyter notebook to analyze global news average tone in Pandas
    * This will create China/US/UK's global news tone with special topic
* Run `theme_spark.ipynd` in jupyter notebook to analyze global news average tone in Spark framework
    * This will create China/US/UK's global news tone with special topic

## Indexing

1. [Input Data](#Input-Data)
2. [Merging Dataset](#Merging-Dataset)
3. [Filtering Theme](#Filtering-Theme)
4. [Cleaning Data](#Cleaning-Data)
5. [Calculating worldwide Average Tones of News from China, US, UK](#Calculating-worldwide-Average-Tones-of-News-from-China,-US,-UK)
6. [Filtering Result](#Filtering-Result)
7. [Visualizaing Worldwide Average Tone](#Visualizaing-Worldwide-Average-Tone)


## Input Data