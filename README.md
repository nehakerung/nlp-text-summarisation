# Summarisation of News Articles

This project is an text summarisation model specifically trained on a dataset of news articles and reference summaries.
It explores transformer based models BART and DistilBART to generate accurate summaries. It includes full preprocessing, dataset handling, model fine-tuning, and evaluation of models.

## Instructions to run code
All instructions and code paths depend on whether you're running locally or in a cloud notebook environment such as Google Colab.

1. Local Notebook / IDE

    * Make sure Python and pip are installed
    * Install required libraries: `pip install -r requirements.txt`
    * Open and follow the notebook, main.ipynb, sequentially

2. Google Colab

    * Open and follow the notebook, main.ipynb, sequentially

#### About Dataset
Thehe original dataset is included on the repo.

If you would like to use your own dataset, a compatible folder layout would look like the following; where the number of articles coresponds with the same number summary.
```
dataset
├── Articles
│   └── 001.txt
|   ├── 002.txt
|   ...
|   └── 511.txt
└── Summary
    └── 001.txt
    ├── 002.txt
    ...
    └── 511.txt
```
Please bear in mind, in colab you will have to take several extra steps:
* Save the dataset folder as a zip file
* Upload to the current colab workspace as a zip file
* Unzip via following

```
!unzip /content/dataset.zip
```
## Model choice
distilBART was initially used
BART