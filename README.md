

## Nargo version:
Nargo version 0.36.0

## bb version:
bb --version   

0.58.0%

## About

Why does `main` throw this error, when there are no slices or references (as far as I can tell) in the `RuntimeBigNum` type?

```
error: Only sized types may be used in the entry point to a program
    ┌─ src/main.nr:248:13
    │
248 │ fn main(_x: RuntimeBigNum<18, 2048>) {
    │             ----------------------- Slices, references, or any type containing them may not be used in main, contract functions, or foldable functions
```