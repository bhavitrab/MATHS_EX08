Algorithm for QR Decomposition
Aim:
To implement QR decomposition algorithm using the Gram-Schmidt method.

Equipment’s required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner
Algorithm:

Initialize the matrix Q and u

The vector u and e is given by

𝑢
1
=
𝑎
1
u
1
	​

=a
1
	​

𝑢
2
=
𝑎
2
−
(
𝑎
2
⋅
𝑒
1
)
𝑒
1
u
2
	​

=a
2
	​

−(a
2
	​

⋅e
1
	​

)e
1
	​

𝑢
3
=
𝑎
3
−
(
𝑎
3
⋅
𝑒
1
)
𝑒
1
−
(
𝑎
3
⋅
𝑒
2
)
𝑒
2
u
3
	​

=a
3
	​

−(a
3
	​

⋅e
1
	​

)e
1
	​

−(a
3
	​

⋅e
2
	​

)e
2
	​

𝑒
1
=
𝑢
1
∥
𝑢
1
∥
e
1
	​

=
∥u
1
	​

∥
u
1
	​

	​

𝑒
2
=
𝑢
2
∥
𝑢
2
∥
e
2
	​

=
∥u
2
	​

∥
u
2
	​

	​


Obtain the Q matrix

𝑄
=
(
𝑒
1
  
∣
  
𝑒
2
  
∣
  
…
  
∣
  
𝑒
𝑛
)
Q=(e
1
	​

∣e
2
	​

∣…∣e
n
	​

)

Construct the upper triangular matrix R

𝑅
=
[
𝑎
1
⋅
𝑒
1
	
𝑎
2
⋅
𝑒
1
	
𝑎
3
⋅
𝑒
1


0
	
𝑎
2
⋅
𝑒
2
	
𝑎
3
⋅
𝑒
2


0
	
0
	
𝑎
3
⋅
𝑒
3
]
R=
	​

a
1
	​

⋅e
1
	​

0
0
	​

a
2
	​

⋅e
1
	​

a
2
	​

⋅e
2
	​

0
	​

a
3
	​

⋅e
1
	​

a
3
	​

⋅e
2
	​

a
3
	​

⋅e
3
	​

	​

	​

Program:
Gram-Schmidt Method







Output

Result
Thus the QR decomposition algorithm using the Gram-Schmidt process is written and verified the result.
