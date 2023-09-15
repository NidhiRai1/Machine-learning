
# Machine-learning
ng

//WHAT IS ML?
------SUPERVISE LEARNING - LEARN INPUT TO OUTPUT MAPPING , LEARNIGN ALGORITHUM LEARN FROM KEY EXAMPLE GIVEN BY THE PROGRAMMER
*INPUT DATA ALONG WITH OUTPUT IS PROVIDED HERE 
*OUTPUT IS PRIDECTED BY SUPERVISED LEARNING
 TYPE OF SUPERVISE LEARNIGN - 
 1.REGRESSION - PREDICTION CAN BE DONE FROM LARGE NO. OF OUTPUT SET .
 iT'S IS USE TO PREDICT CONTINOUS VALUES LIKE - INCOME , AGE , PRICES ETC
  eg ENGLISH (INPUT) ->SPANISH , HINDI , MARATHI , ETC (OUTPUT ) ----- MACHINE TRANSSLATER
2.CLASSIFICATION - IT CAN PREDICT CATAGORY LIKE IS THIS A PICTURE OF CAT OR A DOG (NON - NUMERIC).
IT CAN USE TO PREDICT DISTINT VALUES EG - MALE OR FEMALE , TRUE AND FALSE ETC
 SMALL ONE OF POSSIBLE OUTPUT

 -------UNSUPERVISE LEARNING - IT LEARN FROM THE UNLABALED DATA 
 *ONLY INPUT DATA IS pROVIDEED HERE 
 *HIDEN PATERNS IN THE DATA CAN BE FOUND BY THIS
 EG - DATA PREPROCESSING 
 #TYPES OF UNSUPERVISED LEARNING -
 1.CLUSTERNIG - CALCULATE CLUSTER BASED ON SIMILARITY
 OVERLAPPING , ENCLUSIVE , PROBALISRIC .
EG - SHOPKEEPER PLACING WHITE AND BROWN BREAD TOGHER COZ THEY ARE OF BREAD TYPES

 2.ASSOSIATION - IT FINDS ACCOCIATION BSED ON CO-OCCURANCE 
 EG - PLACING BREAD AND BUTTER TOGETHER COZ THEY ARE COMMENLLY PURCHESED TOGHTER

//LINEAR REGRESSION (SUPERVISED )
traning set - data use to train the model
x - input or feature     and      y - output 
m = no. of traning examples      and (x , y) = single traning eg.            (x^(i) , y^(i)) i th traning example

traning set -> learning algorithum -> x - f -y' (which is estimate prediction of y)
---UNVARIENT LINEAR REGRESSION = y'^(i) = Fw,b (x^(i)) = w*x^(i) + b  where as w , b are parameter to improve the the model by doing traning (weights)
with the different value of w, b we get different f(x) 

//COST FUNCTION - how well the linearn regression model is doing by taking the different pridected and real output 
       y' - y = erroe
       cost function = j(w , b)   = 1/2m[sum from i = 0 -> m [y'^(i) - y^(i)]^2 ]  where m = no. of traning examples
          squared error of cost functions 
goal is to choose w , b such that we minimize cost function

//GRADIENT DESCENT - it is use to minimize any function in case of cost function 
we choose w , b through gradient descent such that it minimize the value of cost function

in case of cost function gradient desent graph will be u shape
     temp_w = w - alpha(differentiate cost function w.r.t w)     = 1/m[          
     temp_b = b - alpha(differentiate coot function w.r.t b)

where their is alpha = learning rate which tells how big small ateps are you talking to reach to the minimum value

//Multiple leniar regression with multiple features and it can be simplifies through vectorization




//problem of fitting in linear regression-
underfitting - not fitting the data very well , high bias , if they have less no. of features
generalization for new examples , fit the tranning set pretty well
overfitting - here error is zero , over fit the data , high variance , if their are too much features then this will hsappen

//ways to avoid the problem of overfitting - 
1.collect more data
2.select features
3.regularization - one of the way to reduce the problem of overfitting by reducing the size (like 0.00001) of some of the features
 in this we have lemda(regularization parameter) which is such that help to fit the data and keep the wj small





--TYPE OF DATA SET ARE :-
1.TRANNING SET - INPUT AND OUTPUT ARE USE TO TRAIN THE MODEL 
2.VALIDATION - CHECK THE PERFORMANCE WHILE TRANNIGN THE DAT AND IF NEEDED THEN FINE TUNE THE PARAMENTER
3.TEST DATA - AFTER THE TRANIGN IS DOEN TEST SET IS CHECK THE PREDICTO=ION HOW CLOSS TO THE OUTPUT DATA 

 --DATA PROCESSING - IT IS DONE TO AMKE THE DATA MORE MEANINGFUL 
--ine hot encoding - it use to give catagorical variable , a numerical value
  ADVANTAGES - 1. convert the catagorical data to a numeriacl value , help to improve the perfrmance of thr model by providing more info.
  
-----unvariable analysis - bar graph , firld plot
-----bivariable analysis - corelational matrix ,
-----time series analysis - 
-----missing data analysis -
-----time series analysis - through out the year

//FEATURE SCALLING - standardize the independent features present in the data in a fixed range. TO SCALE THE 
NORMALIZATION - m value.
             X_{ {scaled }}={X_{i}-X_{text {mean}}}/{X_{{max}} - X_{{min}}}  
SCALAR - LIBRARY 

//HOW TO HANDLE UNBALCED DAATSET - MOST OF REGERESSION MODELING LIKE LOGESTIC NA D DECISION TREE FOCUS ON MAJORITY CLASS ONLY 
        TO HANDLE THIS THEIR ARE TWO WAYS 
  1.SMOT - SYNTHETIC MODELING OVERSAMPALING TECHNIQUE. REPLICATE THE MINORITY CLASS INTITY TO INCRESE THEIR NO. TO MAKE THEM BALANCE
from imblearn.over_sampling import SMOTE
  2.NEARMISS - ALGORITHUM - IT IS AN UNDER SAMPLING TECHNIQUE IN THIS ELIMINATE THE ELEMENT IN MAJORITY CLASS
from imblearn.under_sampling import NearMiss
nr = NearMiss()

--             - relation between dependent nad independent variable .
--linear regression - relations between dependent and independent variable or response and feature variable should be linear.
   //fails for non-linear data craet the problem of underfitting resolve by polynomial regression
--multiple linear regression - feature matrix of n*p and a response mtrix of n row . y(dependent or response) = b + bx + b2x' +b3x''...
      from sklearn.model_selection import train_test_split
import matplotlib.pyplot as plt
import numpy as np
from sklearn import datasets, linear_model, metrics
--polynomial regression - y = w0 + w1x + w2x^2 + ....
--baysian regression - it is a type of liner regression where goal is to estimate the parameters o linear models that 
satisfy the relationship b/w dependent and inde best , effecient when dataset is small but it's time consuming
--quantile regression - Quantile regression constructs a relationship between a group of independent variables and dependent variables. 

