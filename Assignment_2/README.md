## Implementation

#### There are three files:
* viterbi.java
* forward.java
*	bw.java

The **Viterbi** and **Forward** algorithm are implemented in the file with the same name.

Both algorithms receive an HMM with the following information:

* Number of observations
*	Number of states
*	Desired sequence
*	Transition matrix
*	Emission matrix
*	Array with the initial transitions

In the **bw.java** file, the Baum-Welch algorithm is implemtented that allows us to estimate the parameters of a given HMM. 
In order to train this algorithm some sequences are passed.
After indicated threshold value as well as the maximum number of iterations, which serve to finish the calculation of the new transition/emission matrices, these matrices are returned.

## Execution

Compile : `javac 'desired_algorithm'.java`<br />
Run     : `java 'desired_algorithm'`

In order to test these algorithms, some input files are available within the `/examples` folder.

(ex. `javac viterbi.java && viterbi < input_viterbi.txt` )
