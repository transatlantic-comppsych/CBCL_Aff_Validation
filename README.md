# CBCL_Aff_Validation

Code for the manuscript on validation of CBCL-Aff on three datasets (ABCD, HBN, BHRC)

# Authors

[Marie Zelenina](https://github.com/mariezelenina)

Daniel S. Pine

[Argyris Stringaris](https://github.com/Argyris36)

[Dylan M. Nielson](https://github.com/Shotgunosine)

# Important links

## Preregistrations
- [Validation of CBCL-Aff on ABCD data](https://osf.io/a93ts/).
- [Validation of CBCL-Aff on HBN and BHRC data](https://osf.io/vw5ek/).

# Abstract

This is the repostory for the code used for the manuscript "Validation of CBCL depression scores of
adolescents in three independent datasets". Depression is a common and deadly disease which originates in childhood. The Adolescent Brain Cognitive Development study (ABCD) provides an attractive tool to study depression in children and adolescents. The only continuous measure of depression provided in ABCD is the parent-report Child Behavior Checklist’s DSM-5-Oriented Affective Problems scale (CBCL-Aff). It is important for depression research in
the ABCD dataset that the CBCL-Aff is a valid measure of depression in this age group. We, therefore, tested the sensitivity and specificity of
the CBCL-Aff for depression in the ABCD data. CBCL-Aff agreed with parent-report of children’s symptoms but disagreed with child self-report
of symptoms. To resolve the disagreement between parents and their children, we further confirmed our results in two independent datasets
which included data from children aged 9-12: the Healthy Brain Network (HBN) and the Brazilian High Risk Cohort Study (BHRC). Both HBN
and BHRC provided clinician-report depression diagnoses, which we used as a gold standard. CBCL-Aff successfully predicted clinician-report di-
agnoses, supporting its validity as a continuous measure of depression.

# How to run the code

All preprocessing and analyses were conducted in Python, using Jupyter Notebooks.
This directory has 9 .ipynb files, one for each dataset and hypothesis:

1. ABCD - child-report:
- ABCD_child_Hyp1.ipynb
- ABCD_child_Hyp2a.ipynb
- ABCD_child_Hyp2b.ipynb

2. ABCD - parent-report
- ABCD_parent_Hyp1.ipynb
- ABCD_parent_Hyp2a.ipynb
- ABCD_parent_Hyp2b.ipynb

3. HBN - clinician-report
- HBN_Hyp1.ipynb
- HBN_Hyp2a.ipynb

4. BHRC - clinician-report
- BHRC_Hyp1.ipynb
- BHRC_Hyp2a.ipynb
- BHRC_Hyp2b.ipynb

Hyp1 = ***Sensitivity***, the ability of CBCL-Aff to differentiate between depressed and not depressed children.

Hyp2a = ***Specificity***, the ability of CBCL-Aff to differentiate between depressed children and children w/o depression but with another form of psychopathology (ADHD/anxiety).

Hyp2a = ***Strict Specificity***, the ability of CBCL-Aff to differentiate between children with depression and w/o comorbidities and children w/o depression but with another form of psychopathology (ADHD/anxiety).

# Where/how to get the data

## 1. ABCD

Data is shared through the [NIMH data archive](https://nda.nih.gov/abcd/). A tutorial on how to access and download the data is available [here](https://nda.nih.gov/tutorials/abcd/query_and_download.html?chapter=querying-abcd). Prior to downloading the data, the user needs to create an account on the NDA website and request permission.

## 2. HBN

The link to the data and instructions for download are available [here](http://fcon_1000.projects.nitrc.org/indi/cmi_healthy_brain_network/Pheno_Access.html). 

## 3. BHRC

Instructions for requesting the data are available [here](https://osf.io/ktz5h/wiki/home/). [Request form](https://docs.google.com/forms/d/e/1FAIpQLSebaD9yy4QUHxqOKY-Zof6X_EMoq0atnLvsAQfQ9VsmQh63lw/viewform).

# How to run the code

Run each Jupyter notebook block by block. Please submit an issue in this repository or reach out to [Marie Zelenina](https://github.com/mariezelenina) or [Dylan Nielson](https://github.com/Shotgunosine) with questions.

## How to install dependencies

We use the following libraries: 

### [pandas](https://pandas.pydata.org/)

Data analysis and manipulation, used for creting and manipulation dataframes.

[Installation instructions](https://pandas.pydata.org/getting_started.html), [Advanced installation instructions](https://pandas.pydata.org/docs/getting_started/install.html).

Installing with pip:

  pip install pandas

Installing with conda:

  conda create -n name_of_my_env python
  source activate name_of_my_env
  conda install pandas

### [numpy](https://numpy.org/)

Scientific computing in python.

[Installation instructions](https://numpy.org/install/)

Installing with pip:

  pip install numpy

Installing with conda:

  conda create -n my-env
  conda activate my-env
  conda config --env --add channels conda-forge
  conda install numpy

### [matplotlib](https://matplotlib.org/)

A library for producing plots.

[Installation instructions](https://matplotlib.org/stable/users/installing/index.html)

Installing with pip:

  pip install matplotlib

Installing with conda:

  conda install matplotlib

### [itertools](https://docs.python.org/3/library/itertools.html)

Functions creating iterators for efficient looping

This is a python standard library.

### [scikit-learn (sklearn)](https://scikit-learn.org/stable/)

A ML library, for analysis methods such as the AUCROC function and the confusion matrix generator. 

[Installation instructions](https://scikit-learn.org/stable/install.html#installation-instructions).

Installing with pip:

  pip install -U scikit-learn

Installing with conda:

  conda create -n sklearn-env -c conda-forge scikit-learn
  conda activate sklearn-env

### [scipy](https://scipy.org/)

A library for Fundamental algorithms for scientific computing in Python, for sttaistical analysis. 

[Installation instructions](https://scipy.org/install/).

Installing with pip:

  python -m pip install scipy

Installing with conda:

  conda install scipy
