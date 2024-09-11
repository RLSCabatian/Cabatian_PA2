Normalization Problem
``` python
#Import numerical python Library
import numpy as np

#Create random 5x5 array
X = np. random. rand(5, 5)

#Function for Normalized Values
Z = (X - X.mean()) /X.std()

#save Normalized values as X_nomatized. ny
np. save("X_normalized.npy", Z)

#Print X and Z
print ("Original Value: \n", X, "\n Normalized Value: \n", Z)

#end

Original Value: 
 [[0.46086187 0.84715866 0.25929357 0.93914511 0.96556181]
 [0.41596598 0.83260649 0.18402485 0.51945112 0.51266944]
 [0.55735762 0.87197792 0.58047002 0.72199439 0.10709104]
 [0.29896503 0.83882289 0.46014752 0.32504504 0.65463942]
 [0.35445968 0.092665   0.48369713 0.77633538 0.30893073]] 
 Normalized Value: 
 [[-0.2885077   1.21936853 -1.0753122   1.5784297   1.68154503]
 [-0.46375493  1.16256538 -1.36911718 -0.05980963 -0.08628134]
 [ 0.08815514  1.31624838  0.17837239  0.73080058 -1.66942168]
 [-0.92045809  1.18683059 -0.29129614 -0.81865701  0.46788625]
 [-0.70383948 -1.7257325  -0.19937223  0.94291595 -0.88155782]]
```
Divisible by 3 Problem
``` python
#Import numerical python Library
import numpy as np

#Make an array with the first 100 positive numbers in it
A = np.array(np.arange (1,101,1))

#Make the array 10 by 10 in size
A.resize (10,10)

#Creates a new array and squares each entry on its own
Squared_A = np.square (A)

#Keeps track of each Squared A element that is divisible by three.
Div_by_3 = Squared_A[A&3==0]
np. save ('div_by_3.npy', Div_by_3)

#Print
A

array([[  1,   2,   3,   4,   5,   6,   7,   8,   9,  10],
       [ 11,  12,  13,  14,  15,  16,  17,  18,  19,  20],
       [ 21,  22,  23,  24,  25,  26,  27,  28,  29,  30],
       [ 31,  32,  33,  34,  35,  36,  37,  38,  39,  40],
       [ 41,  42,  43,  44,  45,  46,  47,  48,  49,  50],
       [ 51,  52,  53,  54,  55,  56,  57,  58,  59,  60],
       [ 61,  62,  63,  64,  65,  66,  67,  68,  69,  70],
       [ 71,  72,  73,  74,  75,  76,  77,  78,  79,  80],
       [ 81,  82,  83,  84,  85,  86,  87,  88,  89,  90],
       [ 91,  92,  93,  94,  95,  96,  97,  98,  99, 100]])
