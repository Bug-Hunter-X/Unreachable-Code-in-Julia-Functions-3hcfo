# Unreachable Code in Julia

This repository demonstrates a subtle bug in Julia related to unreachable code within functions.  While not strictly an error, the presence of unreachable code can indicate logical flaws that may be harder to detect.

## The Bug

The `bug.jl` file contains a function with an unreachable `return` statement.  Because Julia does not issue a warning or error for this scenario, it's easy to introduce these kinds of logical flaws into the code.

## The Solution

The `bugSolution.jl` file offers improved code that addresses the issue.  This includes restructuring the code to prevent unreachable code and improving readability. 

This example highlights the need for careful code review and potentially incorporating static analysis tools to detect potential problems.