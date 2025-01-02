# Lua Nested Table Iteration Bug

This repository demonstrates a subtle bug in Lua related to nested table iteration using `pairs`.  When iterating over a nested table and modifying it (even indirectly) during the iteration, the `pairs` iterator may skip elements.

The `bug.lua` file contains the problematic code. The `bugSolution.lua` file provides a corrected version. 

This bug is particularly uncommon because it's tied to specific patterns of table modification during iteration in nested functions.