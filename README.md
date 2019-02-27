# Named Entity Evaluation as in SemEval 2013 task 9.1

This repository contains my own implementation of Named-Entity Recognition evaluation metrics as defined by the SemEval 2013 9.1 task.

This metrics go belong a simple token/tag based schema, and consider diferent scenarios based on wether all the tokens that belong to a named entity were classified or not, and also wether the correct type was assigned

You can find a more detailed explanation in the following blog post:

* http://www.davidsbatista.net/blog/2018/05/09/Named_Entity_Evaluation/


## Example:

You can see a working example on the following notebook:

- [example-full-named-entity-evaluation.ipynb](example-full-named-entity-evaluation.ipynb)

Note that in order to run that example you need to have installed:

- sklearn
- nltk
- sklearn_crfsuite

For testing you will need:

- pytest
- coverage

These dependencies can be installed by running `pip3 install -r requirements.txt`

## Test and tests code coverage:

To run tests:

`coverage run --rcfile=setup.cfg -m pytest`

To produce a coverage report:

`coverage report`
