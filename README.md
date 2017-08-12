# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?
A: Naked Twins is used in the same way as "eliminate" and "only choice" have been used.
They are all techniques that allow to reduce the number of possible paths in the search tree towards a possible solution.
This is achieved by eliminating possible values that the varibles in each node can take.
In the specific case of Naked Trees, as it has been explained in the website provided and in the videos, it is about the fact that if two boxes that are peers, contain the same possible two and only two values, then any of the rest of the peers cannot contain those values. We could actually apply Naked Twins to "Triplets" in which if three peers have the same tree values, then their peers cannot have those values... etc.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?
A: I don't think that in the diagonal sudoku we are using constraint propagation, estrictly speaking. When we declare the rules of what peers are to boxes, and what are the solution conditions, we are just adding a new one from the same type as any other, like row peers or column peers. Yes, the diagonal peers are a new constraint, but they are not active techniques applied to states in order to achieve a better or faster solution, or even in order to achieve 'the' solution. Introducing diagonals do change the rules of what the solution is.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solution.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the `assign_value` function provided in solution.py

### Submission
Before submitting your solution to a reviewer, you are required to submit your project to Udacity's Project Assistant, which will provide some initial feedback.

The setup is simple.  If you have not installed the client tool already, then you may do so with the command `pip install udacity-pa`.

To submit your code to the project assistant, run `udacity submit` from within the top-level directory of this project.  You will be prompted for a username and password.  If you login using google or facebook, visit [this link](https://project-assistant.udacity.com/auth_tokens/jwt_login) for alternate login instructions.

This process will create a zipfile in your top-level directory named sudoku-<id>.zip.  This is the file that you should submit to the Udacity reviews system.

