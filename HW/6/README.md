#Computational Thinking <img src="../../Resources/brain.png" width=50px alt="Tick Sheet">


##Instructions
For this computational thinking challenge you should attempt to find a answer to problem set below. The answer to the problem is only part of your response, ***how*** you found the answer is what matters.

Once you can explain the solution you might try to write a computer program to simulate or model the solution. It might even generalise the problem and provide solutions for ***similar*** problems.

##Grading
|Grade|What must I do?|
|-----|---------------|
|D|I will be able to provide an answer to the problem.|
|C|I will be able to provide an answer to the problem, including an explanation of the algorithm / process.|
|B|I will be able to provide a clear explanation of the algorithm I developed to solve to problem.|
|A/A*|I have been able to demonstrate my understanding of the solution to this problem and represented the algorithm using a computer program.|

##The Problem - Ferrying Soliders
####A detachment of **25** soliders need to cross a deep wide river, with no bridge in sight. They spot two boys playing around in a row boat near the shore. They notice two children playing in a rowboat by the shore.
![Ferrying soldiers](../../Resources/ferrying.png)
####The boat is so tiny, however, that it can only hold the two children *or* one of the soliders. How can the soliders get across the river and leave they children in joint posession of the boat? How many times does the boat need to pass from shore to shore in your solution?

###Rules:
- All 25 soliders must end up on the other side of the river.
- The boat can carry one child by themselves, both children or a single solider.
- At the end both children must be with the boat on either shore.

####How many trips from shore to shore must the boat take?
```
29
```
####Explain you algorithm here:
```
To start, two soliders must get in the boat and go to the other side.
One of the soldiers gets off and one stays in the boat.
The one in the boat goes back and picks up another soldier.
This repeats until there are 24 soldiers ont he right side and only one soldier is in the boat.
...
The soldier travels back to the children's side of the shore.
The children travel to the other side and one gets off.
The other child comes back to the other side and swaps places with the last soldier.
The soldier travels to the other side adn swaps places with the other child.
There are now 25 soldiers on the correct side and 1 child on the wrong side.
The child on the wrong side takes the boat used by the last soldier to get back.

```

##Extension
Can you represent the algorithm for this problem using a computer program (any language)?
eg you could show each step in the algorithm using text:

```
in_boat = 0
children = 0
soldiers = 25
rightkids = 2
rightwarriors = 0
while soldiers != 1:
    print ("There are currently {0} soldiers on the right side of the shore".format(rightwarriors))
    print ("There are currently {0} soldiers on the wrong side of the shore".format(soldiers))
    print ("There are currently {0} kids on the right side of the shore".format(rightkids))
    print ("There are currently {0} kids on the wrong side of the shore".format(children))
    print ("There are currently {0} people on the boat".format(in_boat))
    soldiers = soldiers - 2
    print("Two soldiers get in the boat")
    in_boat = 2
    print("They travel to the other side")
    rightwarriors = rightwarriors + 1
    print("One of the two soldiers is dropped off")
    in_boat = 1
    print("The other soldier travels back")
    soldiers = soldiers + 1
    print("and picks up another soldier")
    print("- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - ")
    #the process repeats until only one soldier is left in the boat
    
    #now that there is only one soldier in the boat and two children on the wrong side,
    # the following must happen for the soldier to be on the right side and the children to have the boat at the end.
    
in_boat = 1
print("The last soldier travels back to the wrong side and gets off")
in_boat = 0
print("The two children climb in the boat")
rightkids = 0
children = 2
in_boat = 2
print("One of the children gets off on the other side")
in_boat = 1
print("The other child travels back to the last soldier")
rightkids = 1
print("The soldier swaps places with the child in the boat and goes back to the other side")
rightwarriors = 25
print("The entire detacthment is on the correct shore")
in_boat = in_boat - 1
soldiers = 0
print("The last child gets in the boat and takes it back to his side of the shore")
rightkids = 2
children = 0
print ("There are currently {0} soldiers on the right side of the shore".format(rightwarriors))
print ("There are currently {0} soldiers on the wrong side of the shore".format(soldiers))
print ("There are currently {0} kids on the right side of the shore".format(rightkids))
print ("There are currently {0} kids on the wrong side of the shore".format(children))
print ("There are currently {0} people on the boat".format(in_boat))

#finish

```       

For text based programs like pytohn you should create a new file in you repository
![Add new](../../Resources/new.png)

For anything else (eg scratch), email you teacher with the file and say you've done so in the comments.
