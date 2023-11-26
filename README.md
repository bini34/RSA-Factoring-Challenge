# RSA Factoring Challenge

## Overview

Welcome to the RSA Factoring Challenge project! This project aims to address a critical security vulnerability by factorizing numbers used to encrypt important documents. By successfully factorizing these numbers, we can decode encrypted documents before the target fixes the encryption bug. This is a voluntary project with a potential project grade boost of over 100%.

## Project Details

- **Author:** Julien Barbier
- **Weight:** 1
- **Start Date:** Nov 13, 2023, 6:00 AM
- **End Date:** Nov 27, 2023, 6:00 AM
- **Checker Release Date:** Nov 16, 2023, 6:00 PM
- **Auto Review:** An automatic review will be launched at the deadline.

## Background Context

Before diving into the technical details, start by setting the mood with your favorite background music [here](#)!

We've detected a security loophole in an unsecured network where numbers used to encrypt crucial documents are not always generated using sufficiently large prime numbers. Your mission, should you choose to accept it, is to factorize these numbers quickly before the target fixes the bug, allowing us to decode the encrypted documents.

## Project Scope

This project is entirely optional and offers a project grade boost of over 100%. While participation is not mandatory, it may impact your average positively. The challenge involves factorizing numbers efficiently. The language choice is yours, but the operating system must be Standard Ubuntu 20.04 LTS.

## Resources

To equip you with the necessary knowledge, we recommend reviewing the following:

- [RSA](#)
- [How does HTTPS provide security?](#)
- [Prime Factorization](#)
- [Why RSA?](#)

## Requirements

### General

- Choose a programming language of your preference.
- Operating System: Standard Ubuntu 20.04 LTS.

### Task 0: Factorize all the things! #advanced

Factorize as many numbers as possible into a product of two smaller numbers. The usage of your script should be:

```bash
factors <file>
```

- `<file>`: A file containing natural numbers to factor.
- Each line represents a natural number greater than 1.
- Output format: `n=p*q` (one factorization per line).
- Factors `p` and `q` don’t have to be prime numbers.

#### Example

```bash
$ cat tests/test00
4
12
34
...

$ time ./factors tests/test00
4=2*2
12=6*2
34=17*2
...

real    0m0.009s
user    0m0.008s
sys     0m0.001s
```

### Task 1: RSA Factoring Challenge #advanced

RSA Laboratories states that for each RSA number `n`, there exist prime numbers `p` and `q` such that `n = p × q`. The task is to find these two primes, given only `n`.

The requirements are the same as Task 0, with the following additions:

- `p` and `q` are always prime numbers.
- There is only one number in the files.

#### Example

```bash
$ cat tests/rsa-1
6

$ ./rsa tests/rsa-1
6=3*2
```

## Repository

GitHub Repository: [RSA-Factoring-Challenge](#)

### Files

- [factors](#) (for Task 0)
- [rsa](#) (for Task 1)

## Conclusion

Feel free to explore and have fun with this challenge! Remember, this project is optional, and successful completion can significantly boost your project grade. For any queries, feel free to contact Julien Barbier.

**Copyright © 2023 ALX, All rights reserved.**
