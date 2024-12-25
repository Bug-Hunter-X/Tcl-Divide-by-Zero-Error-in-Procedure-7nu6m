# Tcl Divide-by-Zero Bug

This repository demonstrates a common error in Tcl: a divide-by-zero error that occurs when a procedure doesn't handle zero as input correctly. The `bug.tcl` file contains the buggy code, while `bugSolution.tcl` shows the corrected version.

## Bug Description
The `buggyProc` procedure in `bug.tcl` attempts to divide `$b` by `$a`. However, it doesn't check if `$a` is zero before performing the division.  This leads to an error if the procedure is called with `$a` equal to zero.

## Solution
The corrected version in `bugSolution.tcl` adds a check to handle the case where `$a` is zero, preventing the divide-by-zero error.

## How to Run
1.  Clone this repository.
2.  Execute the scripts using the Tcl interpreter: `tclsh bug.tcl` and `tclsh bugSolution.tcl`.