Algorithm for QR Decomposition
Aim:
To implement QR decomposition algorithm using the Gram-Schmidt method.

Equipment’s required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner


<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/56246d21-b84e-4f62-862d-78832098dd51" />

Program:
```
Gram-Schmidt Method
''' 
Program to QR decomposition using the Gram-Schmidt method
Developed by: BHAVITRA B
RegisterNumber: 212225040047
'''
import numpy as np
def qr_decomposition(A):
    A = np.array(A, dtype=float)
    m,n =A.shape
    Q=np.zeros((m,n))
    R=np.zeros((n,n))
    for j in range(n):
        v=A[:,j]
        for i in range(j):
            R[i,j]=np.dot(Q[:,i],v)
            v=v-R[i,j]*Q[:,i]
        R[j,j]=np.linalg.norm(v)
        Q[:,j]=v/R[j,j]
    return Q,R
A=np.array(eval(input()))
Q,R=qr_decomposition(A)
print("The Q Matrix is")
print("",Q)
print("The R Matrix is")
print( "",R)
```
Output
<img width="1220" height="625" alt="image" src="https://github.com/user-attachments/assets/390ff875-808d-4093-998e-e461e545f9d5" />


Result
Thus the QR decomposition algorithm using the Gram-Schmidt process is written and verified the result.
