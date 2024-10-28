# EX-NO-6-Pseudo-Random-Number

# AIM: 

Implementation of Pseudorandom Number Generation Using Standard library

# DESIGN STEPS:
Step 1: Initialize a Seed

Step 2: Generate the Next Random Number using linear
Congruential Generator (LCG): Xn+1=(aXn+c)

Step 3: Get the no of random numbers to be generated from the user and iterate it

# PROGRAM:
```
Reg no: 212222100049
Name: S.Shanmathi

#include <stdio.h>
//Constants for LCG
#define A 1664525
#define C 1013904223
#define M 4294967296 // 2^32
//Linear Congruential Generator function
unsigned int lcg(unsigned int seed) {
return (A * seed + C) % M;
}
int main() {
unsigned int seed;
int n, i;
printf("**********Pseudorandom number generator**********\n\n");
printf("Enter the seed value: ");
scanf("%u", &seed);
printf("Enter how many random numbers to generate: ");
scanf("%d", &n);
printf("Random numbers:\n");
for (i = 0; i < n; i++) {
seed = lcg(seed);
printf("%u\n", seed);
}
return 0;
}
```

# OUTPUT:
![image](https://github.com/user-attachments/assets/1dade3ea-3b75-402b-ba26-6834c4a23949)

# RESULT:
Hence, pseudorandom numbers are generated successfully
