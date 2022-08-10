# My first beginner code in python. 'Guess a number.'

import random

def guess(x):
    random_number = random.randint(1, x)
    guess = 0
    while guess != random_number:
        guess = int(input(f'Guess a number between 1 and {x}'))
        if guess < random_number:
            print('Higher lad')
        elif guess > random_number:
            print('Lower lad')
    print(f'{random_number} is correct!')

guess(10)
