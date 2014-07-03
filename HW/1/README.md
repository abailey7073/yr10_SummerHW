#Exam Questions <img src="../../Resources/exam.png" width=50px alt="Tick Sheet">

##Instructions
Edit this document and answer the questions in the sections surrounded by ```.

There are **24** marks available and are awarded grades as follows:

|Score|Grade|
|-----|-----|
|<3|U|
|5+|G|
|7+|F|
|9+|E|
|11+|D|
|13+|C|
|15+|B|
|17+|A|
|19+|A*|


##Data Representation

###1 - Why do we represent data using binary when using computers *(1 mark)*

```
Because the machine can only represent data with open and closed electronic circuits.
```
###2 - How would we represent the number 147 in binary? *(1 mark)*
```
010010011
```
###3 - Can you convert the hexadecimal number **b5** to denary, there is a mark for you working. *(2 marks)*
```
181
```
###4 - Here is a function written is **pseudocode**.
```
FUNCTION validUser (users , user)
    FOR x <-1 to LEN(users)
        IF users[x] = user
			RETURN True
		ENDIF
	ENDFOR
	RETURN False
ENDFUNCTION
```

(a) What type of data is **users**? **(1 mark)**
```
string
```

(b) What type of data is returned by this function? **(1 mark)**
```
float
```

##Errors
###6 - This program is supposed to find the mean of a list of numbers and print it out for the user:
```
line1:		tot <- 0
line2:		nums <- [1,6,4,2,5,3]
line3:		FOR x <- to LEN(nums)
line4:			tot <- nums[x]
line5:		ENDFOR
line6:		mean <- tot
line7:		OUTPT mean
```

(a) On which line is there a **syntax** error? **(1 mark)**
```
line 7
```

(b) What is meant by a **syntax** error? **(1 mark)**
```
an error which is caused by misspelling or misunderstanding of code
```

(c) Identify a logical error in the program and suggest how this might be fixed. **(2 marks)**
```
the code does not display the finished calculation
```

(d) Describe and give an example of the 3rd kind of programming error. **(2 marks)**
```
runtime errors are errors caused by user interaction. for example:

imput(int("Type 1 for cookie or type 2 for cake")
if the user types "3" or any other word other than what is described,
the program will crash, because the porgram does not know how to handle the mishap.
```

##Algortithms
###7 - Write an **algorithm** that if given a list of numbers could find the largest. Try to use [pseudocode](http://filestore2.aqa.org.uk/subjects/AQA-GCSE-COMPSCI-W-TRB-PSEU.PDF).
```

```

##Networking
###8 - Research the following methods (*topologies*) for connecting devices to a network. In each case give a description and at least 1 advantage and 1 disadvantage.

**Bus Topology (6 marks)**
```
Describe: A series of nodes and servers are connected to a single cable - A signal from the source is broadcasted and it travels to all workstations connected to bus cable.

Advantages: Easy to set up

Disadvantages: Limits on cable length and connectivity
```

**Ring Topology (6 marks)**
```
Describe: In Ring Topology, all nodes are connected to one another in a way so that they make a closed loop. Each node or server is connected to the two on either side, and it communicates with these two neighbors.

Advantages: Very organised and easing stress on network load

Disadvantages: network packets go through each node on the network, making it slower than star topology.
```

**Star Topology (6 marks)**
```
Describe:   In Star topology, all the servers of network are connected to the central device known as the “hub”.

Advantages: Provides faster performance than bus topology

Disadvantages: If the hub is shut down, the entire network fails.
