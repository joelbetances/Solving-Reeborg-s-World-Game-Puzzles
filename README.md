# Day 6: Solving Reeborg's World Game Puzzles

On Day 6 of my 100 Days of Code challenge with Python, I focused on solving various puzzles in Reeborg's World. This platform allows you to practice programming by guiding a robot through different challenges. Here, I will share the lessons learned, goals achieved, and the code snippets for each challenge.

## Goals for Day 6

By the end of the day, I aimed to achieve the following goals:
1. Define and call Python functions.
2. Solve the Hurdles Loop Challenge.
3. Understand indentation in Python.
4. Master while loops.
5. Complete the Hurdles Challenge using while loops.
6. Jump over hurdles with variable heights.
7. Finish the final project: Escaping the Maze.

## Lessons Learned and Code Snippets

### 1. Defining and Calling Python Functions

**Lesson:** Understanding how to define and call functions in Python.

```python
def turn_right():
    turn_left()
    turn_left()
    turn_left()

# Example usage
turn_right()
move()

### 2. The Hurdles Loop Challenge
Lesson: Using loops to navigate Reeborg through hurdles.

def jump():
    move()
    turn_left()
    move()
    turn_right()
    move()
    turn_right()
    move()
    turn_left()

for step in range(6):
    jump()

### 3. Indentation in Python
Lesson: Learning the importance of proper indentation in Python.

def turn_right():
    turn_left()
    turn_left()
    turn_left()

while not at_goal():
    if front_is_clear():
        move()
    else:
        turn_left()

### 4. While Loops
Lesson: Using while loops to repeat a block of code as long as a condition is true.

while not at_goal():
    if wall_in_front():
        jump()
    else:
        move()

### 5. Hurdles Challenge using While Loops
Lesson: Navigating Reeborg through hurdles with while loops.

def jump():
    turn_left()
    move()
    turn_right()
    move()
    turn_right()
    move()
    turn_left()

while not at_goal():
    if wall_in_front():
        jump()
    else:
        move()

### 6. Jumping over Hurdles with Variable Heights
Lesson: Handling hurdles of different heights.

def jump():
    turn_left()
    while wall_on_right():
        move()
    turn_right()
    move()
    turn_right()
    while front_is_clear():
        move()
    turn_left()

while not at_goal():
    if wall_in_front():
        jump()
    else:
        move()

### 7. Final Project: Escaping the Maze
Lesson: Applying all learned skills to navigate through a maze.

def turn_right():
    turn_left()
    turn_left()
    turn_left()

while not at_goal():
    if right_is_clear():
        turn_right()
        move()
    elif front_is_clear():
        move()
    else:
        turn_left()

### Getting Started

To try out the challenges yourself, visit Reeborg's World and start solving the puzzles. You can use the code snippets provided here as a guide.

### Running the Code
Navigate to the specific challenge on Reeborg's World.
Copy the corresponding code snippet.
Paste the code into the code editor on Reeborg's World.
Run the code to see Reeborg complete the challenge.
