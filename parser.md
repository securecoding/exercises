# Parser

Write a parser in C for a file formatted as follows:

    FROM TO AMOUNT
    FROM TO AMOUNT
    ...

The input is a text file containing the account from which money is transferred, the account to which it is transferred, and the amount of money. The parser doesn't need to output anything, but you should create an internal structure that contains the balance per account after all the transactions have been executed.

For example, take the following input:

    1337 666 1000
    666 1234 888

This should lead to an internal data structure that records the following values:

    1234: 888
    666: 112
    1337: -1000

In class we'll be fuzzing your parser using AFL.
