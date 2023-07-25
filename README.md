# Kistler Cookiecutter for Data Science Team

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._


#### [Project homepage](http://drivendata.github.io/cookiecutter-data-science/)


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5+
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter -c v1 https://github.com/drivendata/cookiecutter-data-science


[![asciicast](https://asciinema.org/a/244658.svg)](https://asciinema.org/a/244658)

### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
├── LICENSE            	<- License in use for this project.
│
├── Makefile           	<- Makefile with commands like `make data` or `make train`
│
├── README.md          	<- The top-level README for developers using this project.
│
├── data               	<- Data for use in this project.
│   ├── output         	<- Final prediction/classification output from the models.
│   ├── pickle         	<- Data stored in the pickle file format.
│   ├── processed      	<- The final, canonical data sets for modeling.
│   ├── protocol       	<- Definition of the data protocol in use.
│   └── raw            	<- The original, immutable data dump.
│
├── docs               	<- A default Sphinx project; see sphinx-doc.org for details
│
├── models             	<- Trained and serialized models, model predictions, or model summaries
│
├── references         	<- Data dictionaries, manuals, and all other explanatory materials.
│
├── requirements.txt   	<- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── reports            	<- Generated analysis as HTML, PDF, LaTeX, etc.
│   ├── csv            	<- Generated data in csv file format to be used in tables in reporting
│   └── figures        	<- Generated graphics and figures to be used in reporting
│
├── setup.py           	<- Makes project pip installable (pip install -e .) so src can be imported
│
├── src                	<- Source code for use in this project.
│   ├── enums          	<- Set of related constants for use in this project.
│   │
│   ├── features       	<- Scripts to build features from data.
│   │
│   ├── models         	<- Scripts to train the models and use them for prediction/classification.
│   │
│   ├── settings       	<- Scripts for general settings accross the project.
│   │
│   ├── utils          	<- Scripts with small helper functions.
│   │
│   └── visualization  	<- Scripts to create exploratory and results oriented visualizations.
│   
├── test_environment.py	<- Script to test the environement for the suitable python version, etc.
│
└── tox.ini            	<- Tox file with settings for running tox; see tox.readthedocs.io
```

## Contributing

We welcome contributions! [See the docs for guidelines](https://drivendata.github.io/cookiecutter-data-science/#contributing).

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests
