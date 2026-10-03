# MRTA Industrial Constraint Test Dataset

This dataset is the test set for the paper *An LLM-Based Framework for Automated MILP Modeling in Dynamic Multi-Robot Task Scheduling*.

It contains 100 test cases covering 10 industrial constraint classes, with 10 cases per class:

1. Robot Release Time
2. Task Completion Precedence
3. Due Date
4. Task Release Time
5. Subtask Start Time Window
6. Task Delivery Time Window
7. Minimum Time Lag
8. Synchronous Task Completion
9. Inter-task Subtask Precedence
10. Global Task Precedence

## Files

The `json` directory contains one file per constraint class. The `all_100_cases.json` file combines all 100 test cases.

## Fields

Each test case contains:

- `constraint`: Natural-language descriptions of five foundational scheduling constraints and one scenario-specific constraint.
- `formula`: Complete LaTeX MILP formulation of the six constraints.
- `code`: Complete Python-Gurobi implementation of the scheduling model.

Cases in `all_100_cases.json` additionally contain a `class` field with a value from `C1` to `C10`.
