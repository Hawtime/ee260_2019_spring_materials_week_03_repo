---
title: Lab2 Report
author:Billy Paulo
partner:Geordan Alferos
date:2/3/19
---
# Task Number 1-1

The objective of this task was to create a 4 bit number in binary format (00010 for two) and have the number chosen displayed on a 7-segment display on out Nexys4 DDR board.
The first portion of the verilog code defines the inputs/outputs that will be used in our project. The only input needed for this task is the input (test) that will hold our 4 bit number while (seg), our output will have nine "cases" that tie to the 7-segment display. Each of the nine states will be linked to different configurations of the 7-segment display leading to a number being displayed. An example is the first state, (seg 0), is linked to the configuration 0000001, which in negative logic would light up each of the different sections besides the last one displaying a 0. At the end of the cases we have a default case which tells the display to turn everything off if we are not trying to display a number between one and nine. 

One problem we encountered during the task was issues with notation. We constantly struggled with notation issues during this task and had to scrap our code a few times and start fresh in order to find out exacly where we were going wrong. After during some research online we found where our problems were coming from, mostly due to having comma's in the wrong places and too many semicolens. Another problem we started out with was we had no clue on where to start with this problem. After referring to the previous lab section and doing some research online we found a good bases to start our code.


# Task Number 3-1

The objective of this task was to create a 4 bit ripple carry adder which would add two 4 bit numbers together and produce the result.
The code is designed to take 4 bit numbers and add them together while taking into account factors such as carry over values. An example is adding 0011 and 0001 resulting in 0100. This works by checking to see if there will be a carry over from the previous addition using the output cout in the code. This gate checks to see if one of the conditions have been met to have a carry over, normally from adding two or more one bit numbers. If one of the conditions have been met it will add 1 to the current adder and move on to the next adder. This continues until the last adder which will result in either a four or five bit number, if the last adder had a carry over bit it will result in the final number being five bits.
  
One of the largest issues with this task was trying to figure out how to implement the carry over bit. We did not know exactly how to tell when we would have that extra bit, but after refering to the labs logic tables it started to make sense in where that extra bit would appear and from there it was easy to account for it into the adder. Being able to understand the logic table is important because it tells you everything you need to know about the function, you just need to know how to read it. 

# Note
We were not able to perform simulations of the code as we were not able to finish the tasks in lab and when we tried to load simulations at home it resulted in infinite load screens for creating/canceling the simulation. I am also confused about how to read the implementation as when i run it I get 6 boxes with many smaller boxes inside of them. I will try to get these issues solved asap, just wanted to put this note as I know there are some things missings. 
