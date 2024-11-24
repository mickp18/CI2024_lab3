# CI2024_lab3

## Idea

To solve the n-puzzle problem we tried to implement the IDA* (iterative deepening A*) algorithm. We used a State class to represent each state of the puzzle and a Heuristic class to calculate the heuristic cost of each state.
The heuristic we used is the manhattan distance, which proved to be more efficient than the other heuristic we tried to implement. We tried to add some improvements to it like adding the linear conflict heuristic but we eneded up having a computational time much higher than the manhattan distance.
We added also a function to the State class in order to check if the puzzle is solvable, in order to avoid that a random genrated puzzle is unsolvable leading to very high cmoputational times.

## Results

- With 3x3 grids the algorithm performs fine and has computational times of few seconds.
- With higher dimensions the computational time proved to be unpredictable, since it depends a lot on how the puzzle was generated, leading to cases where a 6x6 puzzle is solvable faster than a 4x4.




 ## Credits

 The code was developed in collaboration with my [friend](https://github.com/GioSilve).

 Some of the test samples and ideas for creating the State class were inspired by the code of our friend  [Dennis Gobbi](https://github.com/GDennis01/CI2024_lab3/blob/master/n-puzzlev2.ipynb)