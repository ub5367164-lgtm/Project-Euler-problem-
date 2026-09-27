# Project-Euler-problem-
Solution for project Euler problem in python
# Project Euler - Problem 1: Multiples of 3 or 5

## Problem Statement
If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6, and 9. The sum of these multiples is 23.

## Solution Approach

We check every number below 1000 and add it to the total if it is divisible by 3 or 5.


def solve_problem(limit):
    total_sum = 0

    # Check every number below the limit
    for number in range(1, limit):

        # Check if the number is divisible by 3 or 5
        if number % 3 == 0 or number % 5 == 0:
            total_sum += number

    return total_sum


# Set the limit to 1000
limit = 1000

# Calculate the sum
result = solve_problem(limit)

# Display the answer
print(f"The sum of all multiples of 3 or 5 below {limit} is: {result}")

Output

The sum of all multiples of 3 or 5 below 1000 is: 233168

