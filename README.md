# EXP. NO: 05
# DATE:
# <p align="center">Markov Process</p>


# Aim : 

![image](https://user-images.githubusercontent.com/104613195/170176804-7a25305b-c5e3-4b93-8201-8ebbe99765cc.png)

# Software required :  

Python

# Theory:

Markov chains, named after Andrey Markov, a stochastic model that depicts a sequence of possible events where predictions or probabilities for the next state are based solely on its previous event state, not the states before. In simple words, the probability that n+1th steps will be x depends only on the nth steps not the complete sequence of steps that came before n. This property is known as Markov Property or Memorylessness. 

Assumptions for Markov Chain :
1. The statistical system contains a finite number of states.
2. The states are mutually exclusive and collectively exhaustive.
3. The transition probability from one state to another state is constant over time.
# Procedure :

![image](https://user-images.githubusercontent.com/104613195/170175685-c6187523-f268-4a3b-b03d-8bbe62647a57.png)



# Program
```
# Developed by : SURYA R
# Reg no:212220230052
import numpy as np
p0=[0.3,0.2,0.5]
p=[[0,2/3,1/3],[1/2,0,1/2],[1/2,1/2,0]]
n=10
for i in range(1,n+1):
    p0=np.multiply(p0,p)
    print("The %d -step probability distribution is"%i)
    print(p0)
```


# Output : 
![maths](https://user-images.githubusercontent.com/75236145/171331091-1156301b-d1c7-4f9e-af57-e18283375723.png)
<br>
![12](https://user-images.githubusercontent.com/75236145/171331099-ca7fdb1c-6350-40e9-8e61-fd5e6096b105.png)

# Results :
Thus,the nth step probability distribution matrix of the three state Markov chain of given matrices are calculated.
