# Expert-Finding

research paper implementaion for Expert Finding on DBLP Bibliography data

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

* DBLP dataset used - [dataset](https://lfs.aminer.cn/lab-datasets/citation/citation-network1.zip)

### Setup

* code uses dataset uploaded to google drive, extracts it and converts it to more interpretable structure. You can do this locally and ignore the *Data Collection* section
* some dependencies will be automatically downloaded.
```
$ pip install pyunpack
$ pip install patool
$ pip install nltk
$ pip install numpy
$ pip install scikit-learn
$ pip install pandas
```

## Running

* Process has been devided into *6* sections:
  * *Data Collection* - fetches data from google drive, converts it from raw text to json object and saves as 'citation-converted.JSON' to drive
  * *Pre-Processing* - does all the pre-processing to title and abstract fields and adds new field 'text' to json object. saves as new file 'citation-updated.JSON' to drive.
  * *Tf-idf* - tf-idf implementation, keywords extraction, new files to drive 'corpus.txt' and 'docs_keywords.json'
  * *Common Computations* - common work needed for both model implementations
  * *Model 1* - Model 1 implementation, top 5 recommendation output
  * *Model 2* - Model 2 implementation, top 5 recommendation output
  * *Evaluation* - Precision@n , Recall and F1-score

## Authors

* **Manan Gajjar** - *Initial work* - [emanant](https://github.com/emanant)

## Acknowledgments

* Reference to the statictical language models ULM and WLM : [Formal Models for Expert Finding on DBLP Bibliography Data](https://dl.acm.org/doi/10.1109/ICDM.2008.29)
