# Indonesian News Title Keyword Extraction

## About
This project aim to demonstrate key word extraction from text using tf-idf method. 

The dataset used in this project is "[Indonesia News Title Dataset"](https://github.com/ibamibrahim/dataset-judul-berita-indonesia) which contains more than 90.000 news titles gathered from an online news portal.

## Notebook Structure
This notebook is following this structure:
1. Text Preprocessing: text normalisation, word filtering, lemmatization
2. Simple exploratory data analysis
3. Keyword extraction process using tf-idf

## How TF IDF works?
The basic idea of this proejct is to **determine the importance of each word** in the title. To achieve this, we utilize tf idf scoring which the formula is shown below:

![Credit: https://www.searchenginejournal.com/tf-idf-can-it-really-help-your-seo/331075/](https://cdn.searchenginejournal.com/wp-content/uploads/2019/10/screenshot-1.png)

*Credit: https://www.searchenginejournal.com/tf-idf-can-it-really-help-your-seo/331075/*

Weight is the overall weight of a word in a text. Most important words of a text will have more weight, and vice versa. 

The first term is TF or, term frequency, which determine the ratio of particular word in the current text. For example, if a word "Facebook" is appeared 10 times out of 100 words, then the TF is 0.1

The second term is Inverse Document Frequency, or IDF. Intuitively, this tells us how common a words is appeared accross all documents. Therefore, usually a stopword has a low IDF. Meanwhile, topic words, should have a large IDF because it's unique and only appeared in low portion of documents.

## Authors
If you want to contact the author of this project, reach me through:
- Email: ibamibrahim0 [at] gmail

## Credits:
- [Automated Keyword Extraction from Articles using NLP](https://medium.com/analytics-vidhya/automated-keyword-extraction-from-articles-using-nlp-bfd864f41b34)