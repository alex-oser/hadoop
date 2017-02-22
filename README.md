# Hadoop MapReduce
This repository contains several MapReduce functions that I have written for analyzing large bodies of text such as:
* WordCount: Counts the frequency of every word with an option to toggle case sensitivity using ToolRunner
* AverageWordLength: Finds the average length of every word beginning with the same letter
* SentimentPartitioner: Uses a list of positive and negative words (links below) to perform a sentiment analysis of any text

I wanted to use these programs to confirm the existence of [Zipf's Law](https://en.wikipedia.org/wiki/Zipf's_law) within Shakespeare's collected works and the results are shown below.

---

![alt text](https://github.com/alex-oser/hadoop/blob/master/FrequencyShakespeare.png "Shakspeare Word Frequency")
######This graph shows the frequency of the 100 most common words in the text and as is predicted by Zipf's law the graph approximates a 1/n curve.

---

![alt text](https://github.com/alex-oser/hadoop/blob/master/LogFrequencyShakespeare.png "Shakspeare Word Frequency")
######This graph plots the log rank vs the log frequency for all words appearing in Shakespeare's works and as predicted by Zipf the plot is approximately linear.

The lists of positive and negative words used for sentiment analysis can be downloaded [here](http://www.cs.uic.edu/~liub/FBS/sentiment-analysis.html) and were originally created by professors at the University of Illinois whose work is cited below.

---

Minqing Hu and Bing Liu. "Mining and Summarizing Customer Reviews." 
	Proceedings of the ACM SIGKDD International Conference on Knowledge 
	Discovery and Data Mining (KDD-2004), Aug 22-25, 2004, Seattle, 
	Washington, USA, 

Bing Liu, Minqing Hu and Junsheng Cheng. "Opinion Observer: Analyzing 
	and Comparing Opinions on the Web." Proceedings of the 14th 
	International World Wide Web conference (WWW-2005), May 10-14, 
	2005, Chiba, Japan.
 