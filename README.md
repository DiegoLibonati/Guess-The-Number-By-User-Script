# Guess-The-Number-By-User-Script

## Getting Started

1. Clone the repository
2. Join to the correct path of the clone
3. Use `python GuessTheNumberByUser.py` to execute script

## Description

I made a python script that allows the user to try to guess a number that an AI previously chose. If the user guesses the number that the AI chose he wins.

## Technologies used

1. Python

## Libraries used

1. random

## Galery

![guessthenumberbyuser](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/guessthenumber-0.jpg)

![guessthenumberbyuser](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/guessthenumber-1.jpg)

![guessthenumberbyuser](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/guessthenumber-2.jpg)

## Portfolio Link

`https://diegolibonati.github.io/DiegoLibonatiWeb/#/projects?q=Guess%20The%20Number%20By%20User%20Script`

## Video

In this variable `intents` we will store the total number of attempts it took us to guess a number:

```
intents = 0
```

In `number_range` the user will be asked to choose a range of numbers in which the computer can generate. In `random_number` it will generate a number between 0 and the `number_range` and start asking the user to try to guess:

```
number_range = int(input("Select a number range [If you select 10, the IA will select a random number from 0 to 10]: "))

random_number = round(random() * number_range)

print("¡Random number was generated, try to find the number!")

user_find = int(input("Select a number: "))
```

Until the user guesses it will keep asking him to enter numbers:

```
while user_find != random_number:
    user_find = int(input("Oops, you fail but you can try again. Select a number: "))
    intents+=1
```
