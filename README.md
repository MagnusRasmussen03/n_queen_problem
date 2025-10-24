# N-Queens Solver in Java

This repository contains a Java implementation of the classic **N-Queens problem**, solved using **recursion and backtracking**. The project demonstrates algorithmic thinking, problem solving, and Java programming skills.

## Features

- Finds **all valid solutions** for a board of size `N`.
- Can calculate the **number of solutions** for a range of board sizes.
- Measures **execution time** and **solutions per millisecond**.
- Optional printing of solutions for smaller boards.
- Fully object-oriented design with clear separation of concerns.

## How it Works

The `Solver` class:

1. Uses a **recursive backtracking algorithm** to position queens row by row.
2. Checks legality of queen placement with respect to **columns and diagonals**.
3. Increments the total number of solutions when a valid arrangement is found.
4. Can print solutions in a human-readable format (e.g., `a1 b3 c0 ...`).

## Usage

```java
public static void main(String[] args) {
    Solver s = new Solver();

    // Find and print all solutions for small boards
    s.findAllSolutions(1);
    s.findAllSolutions(2);
    s.findAllSolutions(6);

    // Find number of solutions and execution times for boards from 1 to 12
    s.findNoOfSolutions(1, 12);
}
