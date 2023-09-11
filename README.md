### PCB Trace Impedance Estimation
Author: Jingnan Pan

#### Executive summary

#### Rationale
Why should anyone care about this question?
PCB trace impedance is a very common element and very important in PCB design. The electronics system designers are always trying to design and control the PCB trace impedance as accurate as possible to meet their design goals. So how to accurately estimate the PCB trace impedance will benefit the electronics products a lot. 


#### Research Question
What are you trying to answer?
It is known that the PCB trace impedance was determined by PCB dielectric thickness(h), dielectric constant(er1), trace lower width(w1), trace upper width(w2) and thickness(t). So I will explore the multiple linear regression to estimate the trace impedance by the above features. I will also try a few other ML algorithms to compare the different model performance. A very simple image illustration of these features are shown below.  
          
             w1, w2, t
---------------===--------------------
h, er1

--------------------------------------

#### Data Sources
What data will you use to answer you question?
Use a simulation tool to generate a group of features and the corresponding impedance to these features.


#### Methodology
What methods are you using to answer the question?
Use polynomial to generate higher order of the features, and use multiple linear regression to do the estimation.
Also tried DecisionTreeRegressor and compared the performance of different max_depth of the tree.


#### Results
What did your research find?
Multiple linear regression is a good model to predict the PCB impedance from the critical features above. 


#### Next steps
What suggestions do you have for next steps?
Will need to figure out a way to generate more data to cover other features.

#### Outline of project

- Project Report [https://github.com/panfiona/Capstone/blob/main/Capstone.ipynb]
- Project Summary [https://github.com/panfiona/Capstone/blob/main/Capstone%20Summary_%20Jingnan%20Pan.pptx]
- Project Dataset [https://github.com/panfiona/Capstone/blob/main/MicroStrip_Training_H_ER.csv]


##### Contact and Further Information