## WebAsKB
This repo contains code for our paper [The Web as a Knowledge-base for Answering Complex Questions](https://arxiv.org/abs/1803.06643).
It can be used to train neural question split point models in PyTroch, 
and in particular for the case when we want to run the model over multiple paragraphs for 
each question. Code is included to train on the [ComplexWebQuestions](http://nlp.cs.tau.ac.il/compwebq) datasets.


## Setup

### Setting up a virtual environment

1.  First, clone the repo:

    ```
    git clone https://github.com/alontalmor/webaskb.git
    ```

2.  Change your directory to where you cloned the files:

    ```
    cd webaskb
    ```

3.  Create a virtual environment with Python 3.6

    ```
    virtualenv -p python3 venv
    ```

4.  Activate the virtual environment. You will need to activate the venv environment in each terminal in which you want to use WebAsKB.

    ```
    source venv/bin/activate
    ```
5.  Install the required dependencies.

    ```
    pip3 install -r requirements.txt
    ```
6.  Install pytorch 0.3.1 from their [website](http://pytorch.org/)

7.  Download the data



### Data

By default, we expect source data and preprocessed data to be stored in "data" directory.
The expected file locations can be changed by altering config.py.



## Running 

Now you can do any of the following:

* Run a model on example sentences with `python -m allennlp.run predict`.
* Start a web service to host our models with `python -m allennlp.run serve`.
* Interactively code against AllenNLP from the Python interpreter with `python`.


