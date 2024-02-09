# Scikit Learn

## About the course

This repository is adapted from the one used with the Pearson Publishing (Safari) live webinars:

* Beginner Machine Learning with `scikit-learn`
* Diving Deeper into Machine Learning with `scikit-learn`
* Advanced Machine Learning with `scikit-learn`

Versions of this material are used by other training provided by David Mertz
and [Erudio](http://erudio.one).

If you have attended any webinars or courses using this material, I encourage you
to complete the survey on it at: [Machine Learning with scikit-learn
survey](https://goo.gl/pghpzD).  As folks fill this out, we will fold back the
updated answers into the dataset used in the lessons themselves.

## Installing training materials

Before attending this course, please configure the environments you will need.
Within the repository, find the file `requirements.txt` to install software
using `pip`, or the file `environment.yml` to install software using `conda`.
I.e.:

```bash
# launch conda!
$ conda env create -f environment.yml
$ conda activate erudio.sklearn
(erudio.sklearn) $ jupyter notebook Outline.ipynb
```

Or

```bash
$ python -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
$ jupyter notebook Outline.ipynb
```

A quicker way to do this, is probably to use it within Binder.  Just launch:

> https://mybinder.org/v2/gh/DavidMertz/ML-Webinar.git/HEAD # Pending to remake

## Recommended reading

* [Machine Learning with `scikit-learn`](https://github.com/DavidMertz/ML-Webinar)

* [(Video) Machine Learning with scikit-learn LiveLessons](https://www.oreilly.com/library/view/machine-learning-with/9780135474198/), by David Mertz

* _Hands-On Machine Learning with Scikit-Learn and TensorFlow: Concepts, Tools, 
  and Techniques to Build Intelligent Systems_, by Aurélien Géron

* _Deep Learning with Python_, by Francois Chollet

* _Introduction to Machine Learning with Python: A Guide for Data Scientists_, 
  by by Andreas C. Müller & Sarah Guido 

* _Python Data Science Handbook: Essential Tools for Working with Data_, 
  by Jake VanderPlas

* [Documentation of scikit-learn](https://scikit-learn.org/stable/index.html)


## Conda environment

To share the environment, it is used:  

```shell
conda env export --from-history | grep -v "^prefix: " > environment.yml
```

So only packages that are explicitly requested will be included, and without the
prefix, which is the local folder where the package is installed.

After cloning this repository, you can restore the environment using:

```shell
conda env create -f environment.yml
```
