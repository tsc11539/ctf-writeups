# Wave a flag

**Platform:** picoCTF  
**Category:** General Skills  
**Difficulty:** Easy  

---

## Problem
Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...

---

## Approach
The provided file warm is a binary file. We need to extract useful information from it.
1. Try to run the file using ./warm. Since the file is not executable by default, we need to change its permissions using chmod +x warm.

2. After making it executable, run ./warm and observe the output. The program indicates that more information can be obtained by using a help flag.

3. Following this instruction, run the binary with the -h flag (./warm -h) to display the help message, which reveals the flag.

---

## Commands / Code
```bash
chmod +x warm
./warm
./warm -h
