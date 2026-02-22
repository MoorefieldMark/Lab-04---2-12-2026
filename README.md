# Lab-04---2-12-2026

## Lab Summary

In this lab, we were able to get our first experience working on writing code in Vivado to assign outcomes to the basys boards. We were given a truth table and then asked to find its minterm and maxterm functions and implement those into the pre-structured code. This led to the board following the truth table outputs and turn on a led when the right switches were on. This lab was good practice for finding minterm and maxterm expressions as well as an introduction in how to code outputs.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
 

The 1’s and 0’s can be grouped across edges since there is only a change in one of the variable’s values. This is the same difference as in between cells that do touch.

### Why are the names Sum of Products and Products of Sums?

 

A sum of products means there are a group of ‘and’ gates that lead into one ‘or’ gate. The ‘ands’ are written as multiplication and ‘ors’ as addition which makes ‘ands’ into an ‘or’ the sum of products. The term product of sums is many ‘or’ gates that lead into an ‘and’ gate. This makes it the product of sums.

### Open the test.v file - how are we able to check that the signals match using XOR?

 

XOR returns 0 when both inputs are identical (both 0 or both 1). So led[0] ^ led[1] equals 0 if and only if led[0] and led[1] have the same value. The test checks != 0 to detect a mismatch, meaning if the two signals differ, XOR produces 1, and the test fails. This leads to the error message being thrown.
