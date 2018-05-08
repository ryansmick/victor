# victor
JavaScript Spoiler Detector. To the victor goes the spoils!

This repository is split into two pieces: model selection and browser component. The model selection portion was attempted first to come up with an appropriate model, and the browser component brings that model to the browser to detect spoilers on web pages. The model selection uses a Jupyter notebook titled `model_selection.ipynb` at the root of this repository.

## Model Selection

The model selection uses python 3, and is contained in a Jupyter notebook titled `model_selection.ipynb` at the root of this repository. Running this notebook requires installation of several python packages as well as installation of the Stanford Named Entity Recognizer.

### Setup

Run the following commands:

```
# Move to project directory
$ cd PATH_TO_PROJECT

# Install python packages
$ pip install -r requirements.txt

# Install Stanford Named Entity Recognizer (NER)
$ curl -o stanford-ner.zip http://nlp.stanford.edu/software/CRF-NER.html#Download

# Unzip the NER
$ unzip stanford-ner.zip
```

*NOTE: Use of the NER requires a java installation. You can run `java -version` in the command line to see if you have java installed. If no text appears when running that command, java is not installed. Simply follow installation instructions for your machine before moving on*

### Usage

Simply run `jupyter notebook` from the command line. When your browser opens, navigate to `model_selection.ipynb` to view the notebook.
