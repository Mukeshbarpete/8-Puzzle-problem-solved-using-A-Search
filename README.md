# 8-Puzzle-problem-solved-using-A-Search
Implement a search algorithm for solving the 8-puzzle problem with
following assumptions.
 f(n) = g(n) + h(n)
A. . g(n) = least cost from source state to current state so far.
B. Heuristics
a. h1(n) = 0.
b. h2(n) = number of tiles displaced from their destined position.
c. h3(n) = sum of Manhattan distance of each tiles from the goal
position.
d. h4(n) = Devise a heuristics such that h(n) > h∗ (n).
1. Observe and verify that better heuristics expands lesser states.
2. Observe and verify that all the states expanded by better heuristics should
 also be expanded by inferior heuristics.
3. Observe and verify monotone restriction on the heuristics.
4. Observe un-reachability and provide a proof.
5. Observe and verify whether monotone restriction is followed for the
 following two Heuristics:
 Monotone restriction: h(n) <= cost(n,m) + h(m)
a. h2(n) = number of tiles displaced from their destined position.
b. h3(n) = sum of Manhattan distance of each tiles from the goal
e. position.
6. Observe and verify that if the cost of the empty tile is added (considering
 empty tile as another tile) then monotonicity will be violated
Solution
1. Algorithm:
STEP 1: Ask user to enter input manually or randomize.
STEP 2: Take the initial state of the puzzle from user.
STEP 3: Check whether the puzzle is solvable or not.
STEP 4: If puzzle is NOT solvable, output printing “Puzzle is not solvable with in
given time also computing the number of steps which has been visited”.
STEP 5: If puzzle is Solvable, we are counting the number of steps, finding the depth, 
printing the path required to reached the goal state using the different heuristic value 
h1, h2,h3,h4.
