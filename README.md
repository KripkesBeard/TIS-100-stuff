# TIS-100
[TIS-100](http://www.zachtronics.com/tis-100/) is an assembly-like programming game developed by Zachtronics, creators of the games [SpaceChem](http://www.zachtronics.com/spacechem/), [Infinifactory](http://www.zachtronics.com/infinifactory/), [Shenzhen I/O](http://www.zachtronics.com/shenzhen-io/), among others. It consists of a DOS-like interface that presents programming puzzles using a unique, low level programming language made up of interconnected terminals equipped with an accumulator, a back up register, and a very limited amount of space to use an even more parsimonious instruction set to maniupluate data passed between the nodes. TIS-100 is an amazing game that really forces you to think abstractly about low level memory management. 

The game is divided into puzzles normally ask you to take some set of numerical data and manipulate it in a certain way. The game also has threeoptimization benchmarks: cycle count, node use count, and instructions used count. Each node has a set amount of space for constructions, nodes are connected to nodes next to them on the grid, and each instruction takes up some amount of cycles when executed. The three benchmarks are obviously not always possible to optimize at the same time, so different solutions might have better scores in individual categories. This is, of course, a very accurate implementation of the trade offs of software and hardware design.

Some of the puzzles also have achievements associated with them, which are rewarded for solving the puzzles under extraneous conditions. For example, the first puzzle has an achievement for solving the puzzle in over 100,000 cycles, which is an enormous amount compared to the optimal amount of 83. 

N.B. The source code files contain comments enclosed in standard multi line comment sntax. The game does allow comments, but they are single lined and take up a line in the node's instruction space. Therefore, these multiline comments should be ignored if trying to create a source file for the game. The game does allow comments, but they are single lined and take up a line in the node's instruction space; they are demarkated with '#' and '##' names the program.

# 1) SELF-TEST DIAGNOSTIC 

Optimal for all benchmarks:

[Source Code](https://github.com/KripkesBeard/TIS-100-stuff/blob/master/SELF-TEST%20DIAGNOSTIC/Optimal), [Image](https://imgur.com/NCmY4t5)

Achievement:

[Source Code](https://github.com/KripkesBeard/TIS-100-stuff/blob/master/SELF-TEST%20DIAGNOSTIC/BUSY_LOOP), [Image](https://imgur.com/dZpfDnX)

# 2) SIGNAL AMPLIFIER

Optimal for cycles and achievement:

[Source Code](https://github.com/KripkesBeard/TIS-100/blob/master/SIGNAL%20AMPLIFIER/PARALLELIZE), [Image](https://imgur.com/cQF8CHV)

# 3) DIFFERENTIAL COUNTER

sdf
sdf
sdf

# 4) SINGAL COMPARATOR

sdf





