
# Machine-learning
ng

//WHAT IS ML?
------SUPERVISE LEARNING - LEARN INPUT TO OUTPUT MAPPING , LEARNIGN ALGORITHUM LEARN FROM KEY EXAMPLE GIVEN BY THE PROGRAMMER
*INPUT DATA ALONG WITH OUTPUT IS PROVIDED HERE 
*OUTPUT IS PRIDECTED BY SUPERVISED LEARNING
 TYPE OF SUPERVISE LEARNIGN - 
 1.REGRESSION - PREDICTION CAN BE DONE FROM LARGE NO. OF OUTPUT SET .
 OT SIS USE TO PREDICT CONTINOUS VALUES LIKE - INCOME , AGE , PRICES ETC
  eg ENGLISH (INPUT) ->SPANISH , HINDI , MARATHI , ETC (OUTPUT ) ----- MACHINE TRANSSLATER
2.CLASSIFICATION - IT CAN PREDICT CATAGORY LIKE IS THIS A PICTURE OF CAT OR A DOG (NON - NUMERIC).
IT CAN USE TO PREDICT DISTINT VALUES EG - MALE OR FEMALE , TRUE AND FALSE ETC
 SMALL ONE OF POSSIBLE OUTPUT

 -------UNSUPERVISE LEARNING - IT LEARN FROM THE UNLABALED DATA 
 *ONLY INPUT DATA IS ROVIDEED HERE 
 *HIDEN PATRERNS IN THE DATA CAN BE FOUND BY THIS
 EG - DATA PREPROCESSING 
 #TYPES OF UNSUPERVISED LEARNING -
 1.CLUSTERNIG - CALCULATE CLUSTER BASED ON SIMILARITY
 OVERLAPPING , ENCLUSIVE , PROBALISRIC
EG - SHOPKEEPER PLACING WHITE AND BROWN BREAD TOGHER COZ THEY ARE OF BREAD TYPES

 2.ASSOSIATION - IT FINDS ACCOCIATION BSED ON CO-OCCURANCE 
 EG - PLACING BREAD AND BUTTER TOGETHER COZ THEY ARE COMMENLLY PURCHESED TOGHTER

//LINEAR REGRESSION (SUPERVISED )
traning set - data use to train the model
x - input or feature     and      y - output 
m = no. of traning examples      and (x , y) = single traning eg.            (x^(i) , y^(i)) i th traning example

traning set -> learning algorithum -> x - f -y' (ehich is extimate prediction of y)
---UNVARIENT LINEAR REGRESSION = y'^(i) = Fw,b (x^(i)) = w*x^(i) + b  where as w , b are parameter to improve the the model by doing traning (weights)
with teh different value of w, b we get different f(x) 

//COST FUNCTION - how well the linearn regression model is doing by tqaking the difference pricted and real output 
       y' - y = erroe
       cost function = j(w , b)   = 1/2m[sum from i = 0 -> m [y'^(i) - y^(i)]^2 ]  where m = no. of traning examples
          squared error of cost functions 
goal is to choose w , b such that we minimize cost function

//GRADIENT DESCENT - it is use to minimize any function in case of cost function 
we choose w , b through gradient descent such that it minimize the value of cost function

in case of cost function gradient desent graph will be u shape
     temp_w = w - alpha(differentiate cost function w.r.t w)     = 1/m[          
     temp_b = b - alpha(differentiate sot function w.r.t b)

where their is alpha = learning rate which tells how big small ateps are you talking

//,ultiple leniar regression with multiple features and it cab be simplifies through vectorization




//problem of overfitting -
underfitting - not fitting the data very well , high bias , if they have less no. of features
generalization for new examples , fit the tranning set pretty well
overfitting - here error is zero , over fit the data , high variance , if their are too much features then this will hsappen






 
