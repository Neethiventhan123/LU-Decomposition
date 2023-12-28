# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
1.Read the elements of augmented matrix into array a and b
2.Calculate elements of L and U 
3.Print L and U  
4.Find V by solving LV=B by forward substitution
5.Find X by solving UX=V by backward substitution
6.Print array X as the solution 
```
## Program:
(i) To find the L and U matrix
```python
/*
Program to find the L and U matrix.
Developed by:N.neethiventhan 
RegisterNumber: 212223100038
*/
import numpy as np
from scipy.linalg import lu 
A=np.array(eval(input()))
p,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```pyhton
/*
Program to find the LU Decomposition of a matrix.
Developed by:n.neethiventhan 
RegisterNumber: 212223100038
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu, piv),b)
print(X)
```

## Output:
![image](https://github.com/Neethiventhan123/LU-Decomposition/assets/148514848/0ef2c973-aa75-4c70-ba00-b52693b700cb)

![image](https://github.com/Neethiventhan123/LU-Decomposition/assets/148514848/b46b2586-5275-4745-b4a6-89a2292d8527)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

