# Pitman-Yor Topic Model
## Pitman Yor and Hierarchical Pitman Yor Topic Model

This code follows the process shown in and can either do the Chinese Restaurant Process or Pitman-Yor process 
https://dl.acm.org/doi/pdf/10.1145/1835804.1835890?casa_token=xL1Nq-ytSRkAAAAA:jvlvoRwbAo1zx4nOJLeqUVfflcrrkGJPDfTW31UFUWXl-pW2X6_YTiF5ajkzAvEJ87UTWR1hZkEX

To run the code run **train.py**

python train.py --train test_data.txt --topics 5 --iter 10 --pyp

**pytm.py** contains the code for the class definition of the Pitman-Yor LDA (LPYA) topic model and the LDA topic model (LDA). 

**prior.py** contains the code to generate the proper Gamma and Pitman-Yor priors that are needed to define the classes in pytm.py

**prob.py** contains the code for generating probability distributions when needed. For example, the generative process for Pitman-Yor topic model draws the initial theta from a Dirchelet distribution 

**pyp.py** contains the code for the actual Pitman-Yor and Chinese Restaurant process. This is where the "customers" are assigned to each "table" by the formula's described in the paper.
