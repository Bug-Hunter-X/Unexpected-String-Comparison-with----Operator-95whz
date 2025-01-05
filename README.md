# Tcl Bug: Unexpected String Comparison with == Operator

This repository demonstrates a common, yet easily overlooked bug in Tcl related to the use of the `==` operator for numerical comparison.  Tcl's `==` performs string comparison by default.  This can cause unexpected behavior when comparing numbers that are represented as strings.

## The Bug

The `bug.tcl` file contains a procedure that attempts to compare two numbers. However, due to the inherent string comparison, it produces incorrect results when the input is numbers.

## The Solution

The `bugSolution.tcl` demonstrates the correct approach using the `expr` command to explicitly perform numerical comparison.