# Chapter 1 - Welcome Aboard

## Two Recurring themes
#### The notion of abstraction
Notion of abstraction literally defines that details are not important, you need to understand how to work with the system, we don't need to go into how the system works. 
" Abstractions allow us to be much more efficient in dealing with all kinds of situations. It is also true that one can be effective without understanding what is below the abstraction as long as everything behaves nicely. 
##### BUT
This is where the authors have said beautiful thing:
As long as everyhting works fine and everything goes right in the system, not knowing details of how the system works is fine. 
As soon as you run into a problem and you need to debug or find a solution to the problem then you realise that only knowing how to work with the system does not help. 

" If we never have to combine a component with anything else into a larger system, and if nothing can go wrong with the component, then it is perfectly fine to understand the component only at the level of its abstraction. 

But if we have to combine multiple components into a larger system, we should be careful not to allow their abstractions to be the deepest level of our understanding.

If we don't know the components below the level of their abstractions, then we are at the mercy of them working together without our intervention.

If they don't work together, and we are unable to go below the level of abstraction, we are stuck. 
    ## AND THAT IS THE STATE WE SHOULD TAKE CARE NOT TO FIND OURSELVES IN 


#### Hardware vs Software
Hardware and software are names for components of two parts of a computing system that work best when they are designed by people who take into account the capabilities and limitations of both. 

## Two Very Important ideas

#### Idea 1
All computers be it the fastest or the slowest, most expensive or the cheapest are capable of computing exactly the same things if they are given enough time and enough memory. 

#### Idea 2
It is necessary to transform our problem from the language of humans to the voltages that influence the flow of electrons. 

This transformation is really a sequence of systematic transformations, developed and improved over the last 70 years, which combine to give the computer the ability of carry out what appear to be very complicated tasks. 

In reality, these tasks are simple and straightforward.

## How do we Get the Electrons to Do the work 
     - Problems
     - Algorithms
     - Language
     - Machine (ISA) Architecture
     - Microarchitecture
     - Circuits
     - Devices
    
### 1. The statement of the problem 
Computer is an electronic idiot, it can only do as it is told. 
We describe the problem we wish to solve in Natural Language and it has ambiguity. 

### 2. Algorithm 
The first step in the sequence of transformations is to transform the natural language description of the problem to an algorithm, and in so doing, get rid of the objectionable characterstics of the natural language. 
 - DEFENITENESS : A notion that each step is precisely stated. 
 - EFFECTIVE COMPUTABILITY : Each step can be carried out by a computer. 
 - FINITENESS : A notion that the procedure terminates. 


### 3. The Program
This step is to transform the algorithm into a computer program in one of the programming languages that are available. 
There are two kinds of programming languages, high level languages and low level languages. 
High level lenguages are at a distance from the underlying computer. They are independent of the computer on which the programs wll execute. 

Low Level languages are tied to the computer on which the programs will execute. 

There is generally only one such low-level language for each computer called assembely language for that computer. 


### 4. The ISA
Next step is to translate the program into instruction set of the particular computer that will be used to carry out the work of the program. 

The Instruction Set Architecture (ISA) is the complete specification of the interface between programs that have been written and the underlying computer hardware that must carry out the work of those programs. 

Consider a set of instructions that a computer can carry out --- that is what operations the computer can perform and where to get the data needed to perform those operations. 

Opcode - The term opcode is used to describe the operation
Operand - individual data values. 
data types - The ISA specifies acceptabe representations for operands. 
Addressing modes - The ISA specifies the mechanisms that the computer can use to figure out where the operands are located. 

The number of opcodes, data types, and addressing modes specified by an ISA vary in different ISAs. 

The x86, the ISA used in PC, has more than 200 opcodes, more than a dozen data types, and more than 2 dozen addressing modes. 

The ISA also specifies the number of unique locations that comprises the computer's memroy and the number of individual 0s and 1s that are contained in each location 

Examples of ISA 
- x86
- ARM
- THUMB (ARM)
- POWER
- z/Architecute (IBM)
- SPARC (Oracle)

-----> The translation from a high level language to ISA of the computer on which the program will execute is called compiler. 
The translation from assembely language of a computer to its ISA is done by an assembler.

### 5. Microarchitecture
The next step is the implementation of the ISA, referred to as its microarchitecture. 

### 6. The Logic circuit
The next step is to implement each element pf the microarchitecture out of simple logic circuits. 

### 7. The devices
Each basic logic circuit is implemented in accrodance with the requirements of the particular device technology used. 

