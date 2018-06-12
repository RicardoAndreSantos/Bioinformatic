## Implementation

#### There are five files:
* Main.java
* Global.java
* Local.java
* Matriz.java
* Client_Pesquisa.java
* Client_Comparar.java

All classes are controlled by the class **Main.java**, responsible for launching all the methods and the interface.

```
Global(String s1, String s2)
Local(String s1, String s2)
```
As the name itself indicates the **Global** and **Local** class were implemented to lead global and local alignment.
Within this files there are methods that allow you to initialize the matrix, calculate the scores, make the desired alignment and also print the matrix. In the calculation of the scores, in case of "match" sum 5 otherwise the same value is subtracted.

```
Matriz(String d, int v)
```
This class stores each cell of the matrix with a "string" to identify the direction which gave rise to its cell and its value.

```
procura(String tipo)
```
Within the **Client_Pesquisa.java** class the online order is made, whether this request is a protein or a gene.


## Execution

Compile : `javac Main.java`<br />
Run     : `java Main`

#### At this stage we have 3 alternatives:

* Enter sequences manually

* Search "online"
Lets you choose a protein or gene through a specific identifier, saving its FASTA in a file with the name equal to the identifier.

In the case of the protein, a request is made to (eg Q91502): `https://www.uniprot.org/uniprot/''+param+''. fasta`.

For the gene, the request is sent to (eg A00145): `https://www.ebi.ac.uk/ena/data/view/''+param+''&display=fasta`
(in both cases, the **param** is the identifier).

* Compare sequences from file

For this case, you must have performed the previous step that allows us to obtain the files with the desired content.

To avoid this step you can use the files A00145.txt and A00146.txt that are in the directory `/examples`.
