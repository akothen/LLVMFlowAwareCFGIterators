# Flow-aware-CFG-Iterators
Flow-aware iterators for post- or pre-order basic blocks iteration. The key idea here is that basic block lists in Function class cannot be relied upon to provide the correct order of basic blocks, since they are not required to be in an order to resembles the control flow (basic block terminators do that), and the dominator tree iterators do not take into account the control flow at all. So the iterators implemented in this repo are aware of control flow and iterate over the blocks in pre-or post-order form as required.
