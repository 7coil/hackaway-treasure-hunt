<style>
  * {
    font-family: "Comic Sans MS";
  }
</style>

# Treasure Hunt

Welcome to the Royal Hackaway Treasure Hunt!

## How to play

1. Grab a copy of the [answer sheet](./answersheet.pdf) or go to the front desk to grab a printed copy.
2. Find all 8 QR codes hidden around the building in areas that hackers can visit
    - All QR codes are accessible within walkable hacker areas
    - Avoid entering staff rooms, toilets, storage closets, etc.
3. After finding a QR code, copy/paste the answer into a document _in the numbered order that you find them_
4. **At 10am tomorrow, we will be in the lecture theatre to reveal the answers.**

## Final Answer

To calculate the final answer...

1. Take all digits of your answer and concatenate the digits into a string, in order of the question number (1, 2, 3, 4, 5, 6, 7, 8)

2. Keep iterating the following formula until you are left with a single digit:

3. Add each pair of adjacent numbers, writing down the final digit of the answer (aka mod 10)

4. Each iteration will reduce the length by one. At the end, count up all instances of 6 and all instances of 4 (including any 6s or 4s from your input). `total #6` x `total #4` is the answer.

## Example

Given the answers to the questions (in order) are...

Question | Answer
-------- | --------
Q1       | 67
Q2       | 8301
Q3       | 4

```
 6 7 8 3 0 1 4
  3 5 1 3 1 5
   8 6 4 4 6
    4 0 8 0
     4 8 8
      2 6
       8
```

Digit | Occurances
----- | ----------
4     | 5
6     | 4

Therefore, the final answer is `5x4`, which equals `20`.

Keep your answer to yourselves (or your hacking team) until 10am tomorrow.
We'll reveal the answers then!
