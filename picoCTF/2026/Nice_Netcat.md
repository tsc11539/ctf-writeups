# Nice netcat

**Platform:** picoCTF  
**Category:** General Skills  
**Difficulty:** Easy  

---

## Problem
Description
There is a nice program that you can talk to by using this command in a shell:
Additional details will be available after launching your challenge instance.

---

## Approach
This question teachs you how to use netcat.
1. Launch the challenge instance. You are provided with a command in the following format:
```
$ nc wily-courier.picoctf.net <port>
```
2. Run this command in the shell to connect to the remote service. The program outputs a sequence of integers.
3. Observe that all the integers are within the range 0–127, which corresponds to ASCII values.
4. Convert these ASCII values into characters to obtain the flag.

---

## Commands / Code
```bash
nc wily-courier.picoctf.net <port>

