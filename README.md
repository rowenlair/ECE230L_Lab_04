# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

Today we learned how to represent a truth table, minterms, and maxterm equations in verilog. This is really useful because the naive.v file took a lot more writing than the 
simplified version using min terms and max terms. It also made it easier to debug when we did find an issue. We also learned how to fully represent a truth table on the
basys 3 board and how to test our work using the simulation feature. We also learned how to use the synthesis feature to compare our written truth table to the output logic. 

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
We can group them because only one variable is changing along the axis. 

### Why are the names Sum of Products and Products of Sums?
Sum of Products is named that because of the mathematical interpretation of the logic equations. In SOP you're ORing the minterms with contain ANDs. In POS you're ANDing the maxterms which contain ORs. 

### Open the test.v file – how are we able to check that the signals match using XOR?
It checks if XOR between led[0] which is naive and led[1] or led[2] is equal to 0. If it equals 0 then they're the same, which means everything is going as planned. If it's one then they're different
and something is wrong.

