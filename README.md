# Digit Counter Program

## Overview
This C++ program counts the number of digits in a given integer. 
It takes an input number from the user and outputs how many digits it contains.

## How It Works
- The program reads an integer `n`.
- A loop runs until `n` becomes 0.
- In each iteration:
  - The last digit is removed using division (`n = n / 10`).
  - A counter variable is incremented.
- The final count represents the total number of digits.

## Input
- A single integer value.

## Output
- An integer representing the number of digits.

## Example

Input:
12345

Output:
5

## Corrected Code

```cpp
#include<bits/stdc++.h>
using namespace std;

int main(){
    int n;
    cin >> n;

    int cnt = 0;

    while(n > 0){
        n = n / 10;
        cnt++;
    }

    cout << cnt;
}
