# Tips and Tricks

This repository aims to provide tips and tricks related to Artificial Intelligence, Machine Learning, Deep Learning, Python.
[[_TOC_]]

# FAQ
## How can I perform Advanced Search in Web of Science Database?
- You need to have access Web of Science database. For example, it can be via your student account, university library etc.
- Following is a complex search query
```bash
(
TS = (“Text Mining” OR “Text Analysis” OR “Text Analytics” OR “Text
Intelligence” OR “Text Summarization” OR “Text Classification” OR “Text
Extraction” OR “Text Clustering” OR “Text Visualization” OR “Text Categorization”
OR “Text Retrieval” OR “Web Mining” OR “Document Retrieval”
OR “Document Clustering” OR “Document Classification” OR “Document
Ranking” OR “Document Categorization” OR “Document Summarization”
OR “Information Retrieval” OR “Information Extraction” OR “Knowledge
Retrieval” OR “Knowledge Discovery” OR “Concept Extraction” OR “Natural
Language Processing” OR “Sentiment Analysis” OR “Topic Modeling” OR
“Topic Tracking” OR “Topic Detection”)
AND
ALL = (“Artificial Intelligence” OR “Machine Learning” OR “Deep
Learning” OR “Pattern Recognition” OR “Neural Network” OR “Statistical
Learning” OR “Syntactic Analysis” OR “Semantic Analysis” OR “Sentiment
Analysis” OR “Natural Language Processing” OR “Web Crawling” OR
“Tokenization” OR “Stemming” OR “lemmatisation” OR “Stop Words” OR
“Parts-of-Speech” OR “Bag of Words” OR “TF-IDF” OR “Word Embedding”
OR “N-Gram” OR “Phrase Recognition” OR “Entity Extraction” OR “Named
Entity Recognition”)
)
NOT TI = (“Review” OR “Survey” OR “State-of-The-Art” OR “State of
The Art”)
NOT TS = (“Image Processing” OR “Computer Vision” OR “Object
Recognition” OR “Image Classification” OR “Face Recognition” OR “Object
Detection” OR “Edge Detection” OR “Machine Vision” OR “Image
Segmentation”)
```
- Paste above query into Advanced Search field.
- An example query link can be found [here](https://www.webofscience.com/wos/woscc/summary/11672967-7894-47c1-b645-2bd739b45373-c5fde70d/date-descending/1)
  
## How can I generate word cloud with Python?
- You can use [word_cloud](https://pypi.org/project/wordcloud/) Python package.
- After installing above package, put your text into a file such as **"mytext.txt"**
- Run following command:
```bash
wordcloud_cli --text mytext.txt --imagefile wordcloud.png
```

## How can I use VOSviewer tool to visualize text data in a simple way?
Let's assume that you have a text dataset in Excel file (xlsx). Normally VOSviewer expects a CSV form regarding a dataset from SCOPUS database.
Within this workaround, you are going to provide your text dataset like it is an output from SCOPUS database.
For that purpose, please apply following steps:
- Change column name as **Author Keywords** for the relevant text column in your Excel file.
- Save your Excel file as **csv** format.
- Open VOSviewer.
- Map -> Create -> Create a map based on bibliographic data -> Next.
- Read data from bibliographic database files -> Scopus.
- Locate/upload your csv file.
  - If there is an issue with csv file, please ensure that words in the rows are seperared with "; ". If not, update your file and re-upload.
- Ensure that "Co-occurrence" and "Full Counting" fields are marked.
- Choose threshold.
- Choose number of keywords.
- Finish.
- If everything is fine, you will have a visualization screen.
