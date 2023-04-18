# Machine Learning Tips and Tricks

This repository aims to provide tips and tricks related to Artificial Intelligence, Machine Learning and Deep Learning.
[[_TOC_]]

# FAQ
## How can I use VOSviewer tool to visualize text data in a simple way?
Let's assume that you have a text dataset in Excel file (xlsx). Normally VOSviewer expects a CSV form regarding a dataset from SCOPUS database.
Within this workaround, you are going to provide your text dataset like it is an output from SCOPUS database.
For that purpose, please apply following steps:
- Change column name as **Title** for the text data in your Excel file.
- Add a dummy column with name **AUTHOR KEYWORDS** in your Excel file.
- Save your Excel file as **csv** form.
- Open VOSviewer.
- Map -> Create -> Create a map based on bibliographic data -> Next.
- Read data from bibliographic database files -> Scopus.
- Locate your csv file.
- Ensure that "Co-occurrence" and "Full Counting" fields are marked.
- Choose threshold.
- Choose number of keywords.
- Finish.
- If everything is fine, you will have a visualization screen.
