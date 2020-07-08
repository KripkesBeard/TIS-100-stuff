# TIS-100
[TIS-100](http://www.zachtronics.com/tis-100/) is an assembly-like programming game developed by Zachtronics, creators of the games [SpaceChem](http://www.zachtronics.com/spacechem/), [Infinifactory](http://www.zachtronics.com/infinifactory/), [Shenzhen I/O](http://www.zachtronics.com/shenzhen-io/), among others. It consists of a DOS-like interface that presents programming puzzles using a unique, low level programming language made up of interconnected terminals equipped with an accumulator, a back up register, and a very limited amount of space to use a parsimonious instruction set to maniupluate data passed between the nodes. TIS-100 is an amazing game that really forces you to think abstractly about low level memory management. 

The game is divided into puzzles which ask you to take some set of numerical data and manipulate it in a certain way. The game also has three optimization benchmarks for working solutions to the puzzles: cycle count, node use count, and instructions used count. Each node has a set amount of space for instructions, nodes are connected to the nodes next to them on the grid, and each instruction takes up some amount of cycles to execute. The three benchmarks are obviously not always possible to optimize at the same time, so different solutions might have better scores in individual categories. This is an elegant embodiment of the necessary trade offs of software and hardware design.

Some of the puzzles also have achievements associated with them, which are rewarded for solving the puzzles under extraneous conditions. For example, the first puzzle has an achievement for solving the puzzle in over 100,000 cycles, which is orders of magnitude larger than the optimal count of 83. 

N.B. The source code files contain comments enclosed in standard multi line comment sntax. The game does allow comments, but they are single lined and take up a line in the node's instruction space. Therefore, these multiline comments should be removed when trying to create a source file for the game. 

# 1) SELF-TEST DIAGNOSTIC 

Instructions:

>READ A VLUE FROM IN.X AND WRITE THE VALUE TO OUT.X

>READ A VALUE FROM IN.A AND WRITE THE VALUE TO OUT.A

Optimal for cycles, nodes, and instructions:

[Source](https://github.com/KripkesBeard/TIS-100-stuff/blob/master/SELF-TEST%20DIAGNOSTIC/Optimal), [Image in game](https://imgur.com/NCmY4t5), [Image of finished run](https://imgur.com/Q2KKAvS)

BUSY_LOOP Achievement:

[Source](https://github.com/KripkesBeard/TIS-100-stuff/blob/master/SELF-TEST%20DIAGNOSTIC/BUSY_LOOP), [Image in game](https://imgur.com/dZpfDnX), [Image of finished run](https://imgur.com/C0HDYxx) (N.B., the finished run of this is exponentially less cycles than the source code, it was done by replacing 999 with 9, so instead of a ~1000^5 asymptotic we have ~10^5. The source code would take longer to finish running than the sun has left before it implodes.)

# 2) SIGNAL AMPLIFIER

Instructions:

>READ A VALUE FROM IN.A

>DOUBLE THE VALUE

>WRITE THE VALUE TO OUT.A

Optimal for cycles and PARALLELIZED achievement:

[Source](https://github.com/KripkesBeard/TIS-100/blob/master/SIGNAL%20AMPLIFIER/PARALLELIZE), [Image in game](https://imgur.com/cQF8CHV), [Image of finished run](https://imgur.com/l6M5gKE)

Optimal for nodes and instructions:

[Source](https://github.com/KripkesBeard/TIS-100/blob/master/SIGNAL%20AMPLIFIER/Optimal%20Node%20Instruction), [Image in game](https://imgur.com/r1rRNUT), [Image of finished run](https://imgur.com/BEmUbvf)

# 3) DIFFERENTIAL COUNTER

>READ VALUES FROM IN.A AND IN.B

>WRITE IN.A - IN.B TO OUT.P

>WRITE IN.B - IN.A TO OUT.N



# 4) SINGAL COMPARATOR







