
# Forecasting Future World Events with Neural Networks

## CS542 Midterm Competition

## Introduction

Forecasts of climate, geopolitical conflict, pandemics and economic indicators help shape policy
and decision making. This report aims to give insights into our approach for competing in the
Autocast Competition 2023 and providing a descriptive analysis of the large language models and
methods that were successful as well as those that could be improved. We implement training the
machine learning models on the Autocast dataset and display our findings and improvements to
the Future World Events Prediction task.

## Autocast Dataset

The latest version of the [Autocast dataset can be downloaded here](https://people.eecs.berkeley.edu/~hendrycks/autocast.tar.gz). For more details on how to use the Autocast dataset and news articles, please refer to our short demonstration in `usage.ipynb`.

Each question has the following fields:
  ```json
  {
    "id":                "unique identifier (str)",
    "question":          "question body (str)",
    "background":        "question context/details (str)",
    "qtype":             "question type (str)",
    "status":            "question status (str)",
    "choices":           "choices or possible ranges (List or Dict)",
    "answer":            "question resolution (str or float)",
    "crowd":             "human crowd forecasts over time (List)",
    "publish_time":      "publish timestamp (str)",
    "close_time":        "close timestamp (str)",
    "prediction_count":  "number of crowd predictions (int)",
    "forecaster_count":  "number of crowd forecasters (int)",
    "tags":              "question category (List)",
    "source_links":      "source links from comments (List)"
  }
```

We obtained permission from [Metaculus](https://www.metaculus.com/) to host the dataset on GitHub for research purposes only.

## Running the code

To run the code, open the “autocast_submission.ipynb” file and run the cells as per the model.
The submission.zip file will be created for evaluation. All the data used was taken from the
auxiliary data provided in the CS542 drive. You will need “autocast_questions.json” as well as
“autocast_competition_test_set.json” to replicate our results, and the
“autocast_test_set_w_answers.csv” for evaluation.

