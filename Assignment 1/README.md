## CS6910-DEEP LEARNING ASSIGNMENT 1
                 -ANANTHAKRISHNAN A(ED22S015)
This repository includes the following files:- 


  *CS6910 Assignment-1(CODE ONLY).ipynb*  -This file includes the complete code and the sweeps performed without the outputs.   
  *CS6910 Assignment-1-partial sweep results.ipynb* - This file includes almost 200 number of sweeps performed as output.  
  *CS6910 Assignment-1.ipynb* - This is the original file which includes all the outputs obtained in the jupyter notebook and wandb along with the codes, but due to spain
  constraints, it can only be opened after downloading  the file.
  *feed_forward_NN.ipynb* - This file consists of the implementation of feed forward neural network(forward propogation)
  *train.py* -This file can be used for running the code in the terminal.  
  *CS6910 Assignment 1_old.ipynb*  -Thsi file includes the initial commits (which was changed in between in the jupyter notebook due to continuous kernel issues).    
   
The following packages are used for completing the assignment:-  
  **Numpy** - matrix operations.  
  **WANDB** - performing sweep and analysis results from plots, confusion matrix etc.  
  **scikit-learn** - plotting confusion matrix in the jupyter notebook, test-train-split of dataset.  
  **keras** - importing FASHION-MNIST and MNIST datasets.  
  
*The link to the wandb report of this assignment is given below:-*  
https://wandb.ai/ananthu2014/CS6910_DL_ASS1/reports/CS6910-Assignment-1--VmlldzozNzA2NzAy

Further details about the implementation is given below:-  

### FUNCTIONS USED:-  

1) **pre_processing_data** : This function in train.py performs the following tasks:-  
     Changes the shape of input data and ground truth.  
     Converts the output data into one hot vector form.  
     Creates a validation dataset.  
     Normalizes data.  
     
2) **data_augmentation** : This function in train.py adds a gaussian noise to the train data.  
   mean of gaussian random noise:1  
   variance :0.01  
   
3) **Activation functions and its derivatives** :

   a) sigmoid_function = 1/((1+exp(-z))
   sigmoid_function_dash : This function is the derivative of sigmoid_function    
                         = sigmoid_function(z)x(1-sigmoid_function(z))  
                         
   b) relu_function(z) = max(0,z)  
   Its derivative is given as relu_function_dash(z)    
   
   c) identity_function(z) = z  
   Its derivative is given by identity_function_dash(z)    
   
   d) tanh_function(z) : This denotes the tanh activation function  
   Its derivative is given by tanh_function_dash(z)
   
   e) softmax_function(z) : Since the given problem is a multi-class classification(with 10 labels), we use softmax function for the output layer.  
    Its derivative is given by softmax_function_dash(z)  
    
    Mostly, these activation functions are used in forward propagation and its derivative functions are used in back propagation.  
    
4) **Loss functions** :  

   a) cross_entropy_function : For multi-label problems, cross entropy function is the recommended loss function, which gives a higher penalty in case of misclassifications   
      and therefore, minimizes better.  
      
   b) mean_squared_error_function : Here, Mean squared error loss is used to compare the results obtained with cross entropy loss.  
   
   
     
   
   



  
   

