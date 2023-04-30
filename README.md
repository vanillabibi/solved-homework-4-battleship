Download Link: https://assignmentchef.com/product/solved-homework-4-battleship
<br>
In this program you will be mimicking a game of Battleship. Your game board is a line of 10 slots. You have to implement 3 methods. The following methods must be implemented:

void setBoard(int *)

This method sets up the human’s game board. The method prompts the user for 2 slots to place the “ship”. The program should ensure that the slots are consecutive. In other words, your ship cannot be placed at slot 2 and at slot 6. Since the board has only 10 slots, valid slots are in the range of 0 to 9.

void setComputerBoard(int *)

Exactly the same as the setBoard method except that the position of the computer’s ship is set randomly. The computer’s ship must also be in consecutive slots.

intplayGame(int *, int *)

This method should do the following steps:

<ol>

 <li>Have the computer pick at random a slot to “fire” at. If the slot the computer picked on the human’s board is a ship, a “HIT” message is displayed. If the slot on the human’s board is empty, a “MISS” message is displayed. Print out the computer’s board and the human’s board as described at the bottom of the page.</li>

 <li>After the computer goes, have the human pick a slot to “fire” at. If the slot the human picked on the computer’s board is a ship, a “HIT” message is displayed. If the slot on the computer’s board is empty, a “MISS” message is displayed. Print out the computer’s board and the human’s board as described at the bottom of the page.</li>

 <li>Repeat steps 1 and 2 until there is a winner. The computer wins if both of the human’s ship slots are hit. The human wins if both of the computer’s ship slots are hit.</li>

</ol>




The playGame method returns a 0 if the computer won. The playGame method returns a 1 if the human won.




The computer board is printed off with the following characters: (The human board is printed off similarly)

S – printed off in the slots where the computer’s ship is located.

M – printed off in the slots where the human guessed incorrectly.

H – printed off in the slots where the ship is located and where the human hit.

*  – printed off in all other slots




You can assume the input will always be a positive integer.

<strong>Important: You should use pointer notation when referencing values inside an array as opposed to array notation.  For example, use *ptrToArray instead of array[0] and *(ptrToArray+1) instead of array[1], etc. You will lose 10 points for not following this notation.</strong>

A sample run of the code is below –




Enter 1st position: 4

Enter 2nd position: 5

Computer guesses 9

MISS!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * * S S * * * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S S * * * * * *

Enter guess: 4

You guessed 4

MISS!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * * S S * * * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S S M * * * * *

Computer guesses 4

HIT!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * * H S * * * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S S M * * * * *

Enter guess: 3

You guessed 3

HIT!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * * H S * * * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S H M * * * * *

Computer guesses 7

MISS!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * * H S * M * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S H M * * * * *

Enter guess: 9

You guessed 9

MISS!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * * H S * M * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S H M * * * * M

Computer guesses 3

MISS!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * M H S * M * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S H M * * * * M

Enter guess: 5

You guessed 5

MISS!

Human Board:

0 1 2 3 4 5 6 7 8 9

* * * M H S * M * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S H M M * * * M

Computer guesses 0

MISS!

Human Board:

0 1 2 3 4 5 6 7 8 9

M * * M H S * M * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * S H M M * * * M

Enter guess: 2

You guessed 2

HIT!

Human Board:

0 1 2 3 4 5 6 7 8 9

M * * M H S * M * M

Computer Board:

0 1 2 3 4 5 6 7 8 9

* * H H M M * * * M

Human wins!





