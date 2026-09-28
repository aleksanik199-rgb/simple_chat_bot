
# Simple Chat Bot 🤖

A console application in Kotlin that talks to the user: greets them, guesses their age, counts up to a number and runs a one-question quiz. Built as a learning project on the Hyperskill (JetBrains Academy) platform.

## What it does

1. **Greeting:** the bot introduces itself (name and birth year) and asks for the user's name.
2. **Age guessing:** the user enters the remainders of dividing their age by 3, 5 and 7, and the bot calculates the age with the formula `(rem3 * 70 + rem5 * 21 + rem7 * 15) % 105`.
3. **Counting:** the bot prints every number from 0 to the number the user enters, each followed by `!`.
4. **Quiz:** the bot asks one multiple-choice question and repeats it until the user answers correctly (option 2).

## Project structure

- `SimpleBot.kt` — the whole program, package `bot`. The `main` function calls `greet`, `remindName`, `guessAge`, `count` and `test` in order.

## How to run

1. Install IntelliJ IDEA (or another Kotlin-capable IDE).
2. Clone the repository or copy `SimpleBot.kt` into a Kotlin project.
3. Run the `main` function in `SimpleBot.kt`.
4. Follow the bot's prompts in the console.

## Known limitations

- The program reads input with `Scanner.nextInt()`, so entering text instead of a number crashes it with `InputMismatchException`. Input validation is planned.

## What I practiced

Functions, string templates, `Scanner` input, `for` and `while` loops, `break`, and simple arithmetic with remainders.