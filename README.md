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
jupyter notebook pandas numpy matplotlib scikit-learn scipy

You can create a conda environment with:
`conda env create -p ./env -f environment.yml`