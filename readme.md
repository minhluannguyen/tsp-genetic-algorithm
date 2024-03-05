# Playing around with Genetic Algorithm and the Travelling Salesman Problem

My attempt for solving TSP with Genetic Algorithm.

## Introduction

The Travelling Salesman Problem (TSP) is a classic algorithmic problem in the field of computer science and operations research. It focuses on optimization. In this problem, a salesman is given a list of cities, and must determine the shortest possible route that allows him to visit each city once and return to his original location.

## Genetic Algorithm

A genetic algorithm is a search heuristic that is inspired by Charles Darwin’s theory of natural evolution. This algorithm reflects the process of natural selection where the fittest individuals are selected for reproduction in order to produce the offspring of the next generation.

## Implementation

Each individual in the population will be represented with:
- A "chromosome" with is encoded order of vistied cities.
- A fitness score to determine how good the solution is. In this case, it is $ \frac{1}{\text{total distance}} $ (since the shorter distance the better).

The algorithm will loop through a number of generations, and in each generation:
- Pick out the "survivors" (the best individuals) from the current population.
- Apply crossover and mutation to create the next generation.

This will repeat until a certain of generations. The better an individual is, the more likely it will be picked for reproduction.