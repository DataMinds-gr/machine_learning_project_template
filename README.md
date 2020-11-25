# Machine Learing Project Template

A general skeleton for Machine Learning projects

This project structure was partially influenced by: 

1. [Cookiecutter Data Science project](https://drivendata.github.io/cookiecutter-data-science)

2. [This](https://github.com/cmawer/reproducible-model) github repository


</br>

---

## General Guidlines 

1. Data is immutable
2. Notebooks are for exploration and communication
3. Analysis is a DAG (Directed Acyclic Graph)
4. Build from the environment up
5. Keep secrets and configuration out of version control
6. Be conservative in changing the default folder structure
7. Use virtual environment or docker

</br>

---
## Directories and Files 

</br>

```
├── LICENSE
│
├── (IDE settings dir) <- IDE settings
│
├── .gitignore         <- Ignore files from git
│
├── Makefile           <- Makefile with commands like `make data` or `make train`
│
├── README.md          <- The top-level README for developers using this project.
│
├── TODO               <- TODO file
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│                         
├── setup.py           <- Make this project pip installable with `pip install -e`
│
│
├── run.py             <- Simplifies the execution of one or more of the src scripts 
│
│
├── environment.yml    <- 
│
│
├── config.json        <- 
│
│
├── references/        <- Data dictionaries, manuals, and all other explanatory materials.
│   ├── 	       <-
│   └──                <- 
│
├── docker/            <- Dockerfile and other docker related files
│
├── api/               <- API setup
│   └── app.py         
│
├── data/
│   ├── raw/            <- The original, immutable data dump
│   ├── interim/        <- Intermediate data that has been transformed
│   ├── processed/      <- The final, canonical data sets for modeling
│   ├── predictions/    <- Predictions for evaluation
│   └── external/       <- Data from third party sources
│
├── docs/               <- A default Sphinx project; see sphinx-doc.org for details
│   ├── project/        <- Documentation about the general project scope and final report
│   ├── data/           <- Documentation about datasets
│   └── models/         <- Modeling pipeline documentation
│
├── models/             <- Trained and serialized models, or model summaries
│
├── notebooks/          <- Jupyter notebooks (EDA, Crate Reports)
│   ├── develop         <- Current notebooks being used in development.
│   ├── deliver         <- Notebooks shared with others. 
│   ├── archive         <- Develop notebooks no longer being used.
│   └── template.ipynb  <- Template notebook for analysis with useful imports and helper functions. 
│
├── apps/               <- Shiny / Dash apps
│
│
├── tests/              <- Files necessary for running model tests
│
├── labeling/           <- Gererate targets/labels for the dataset
│
├── reports/            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   ├──      
│   ├── interactive-plots     
│   └── static-plots     <- Generated graphics and figures to be used in reporting
│
│
├── src/                <- Source code for use in this project.
│   │
│   ├── __init__.py     <- Makes src a Python module
│   │
│   ├── data/           <- Scripts to download or generate data
│   │	├── make_dataset.py
│   │   └── 
│   │
│   ├── features/       <- Scripts to turn raw data into features for modeling
│   │	├── generate_features.py
│   │   └── feature_selection.py
│   │
│   ├── models/         <- Scripts to train models and then use trained models to make predictions
│   │   │                 
│   │   ├── train_model.py
│   │   ├── predict_model.py
│   │   ├── evaluate_predictions.py
│   │   ├── model_explainability.py
│   │   └── experiment_N.py
│   │
│   │
│   │
│   ├── helpers/       <- Helper scripts (helper functions, database connect, etc)
│   │
│   │
│   └── visualization/  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
│   
│
└── tox.ini             <- tox file with settings for running tox; see tox.testrun.org
```

----

## Virtual Environment

</br>

Use `venv` and `pip`.

</br>

I. Create a **requirements.txt** file

```
$ pip freeze > requirements.txt
```

II. Create a **virtual environment** based on the requirements.txt file

```
$ python -m venv venv_name
$ source venv_name/bin/activate
$ pip isntall -r requirements.txt
```
---
