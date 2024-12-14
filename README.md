# Subtle String Comparison Bug in Tcl

This repository demonstrates a common, yet subtle, bug in Tcl related to string comparison. The `badproc` procedure in `bug.tcl` incorrectly uses the `==` operator instead of `eq` when comparing strings.  This leads to unexpected results when comparing numeric strings and actual numbers.

The solution, provided in `bugSolution.tcl`, corrects the procedure to use the `eq` operator for accurate string comparison. 

## How to Reproduce
1. Clone this repository.
2. Run `tclsh bug.tcl` and observe the incorrect results.
3. Run `tclsh bugSolution.tcl` and observe the corrected output.
