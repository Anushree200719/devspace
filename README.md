# Even or Odd

## Problem Statement
Given an integer $n$, determine whether the number is Even or Odd.

## 1. Input
A single integer `n` (represented as `long long` in C++ to support 64-bit integers).

### Test Cases
- `8`
- `7`
- `0`
- `-4`
- `-3`
- `1000000000000`

---

## 2. Expected Output
Print `"Even"` if the number is even, or `"Odd"` if the number is odd.

| Input | Expected Output |
| :--- | :--- |
| `8` | `Even` |
| `7` | `Odd` |
| `0` | `Even` |
| `-4` | `Even` |
| `-3` | `Odd` |
| `1000000000000` | `Even` |

---

## 3. Logic
An integer is considered even if it is divisible by 2 with no remainder (`n % 2 == 0`). Otherwise, it is odd.
- In C++, the modulo operator `%` calculates the remainder after integer division.
- For an even integer $n$ (positive, negative, or zero), `n % 2` yields `0`.
- For an odd integer $n$, `n % 2` yields non-zero (`1` for positive, `-1` for negative in C++), satisfying the `else` condition.

---

## 4. Algorithm/Steps
1. **Start**
2. Declare a 64-bit integer variable `n` of type `long long`.
3. Read the integer value from standard input (`cin >> n`).
4. Check if `n % 2 == 0`:
   - If true, print `"Even"` to standard output.
   - If false, print `"Odd"` to standard output.
5. Exit the program with return code `0`.

---

## 5. Source Code

```cpp
#include <iostream>
using namespace std;

int main()
{
    long long n;
    cin >> n;

    if (n % 2 == 0)
        cout << "Even" << endl;
    else
        cout << "Odd" << endl;

    return 0;
}
```

---

# Question 2: Find the Larger Number

## Problem Statement
Given two integers `a` and `b`, find the larger number. If both numbers are equal, display `"Both numbers are equal"`.

## 1. Input
Two integers `a` and `b` (represented as `long long` in C++).

### Test Cases
- `5 23`
- `10 4`
- `-2 -8`
- `7 7`
- `0 -3`

---

## 2. Expected Output
Print the larger number, or `"Both numbers are equal"` if `a` and `b` are equal.

| Input | Expected Output |
| :--- | :--- |
| `5 23` | `23` |
| `10 4` | `10` |
| `-2 -8` | `-2` |
| `7 7` | `Both numbers are equal` |
| `0 -3` | `0` |

---

## 3. Logic
Compare the two numbers `a` and `b` using conditional statements:
- If `a > b`, `a` is strictly greater than `b`, so output `a`.
- Else if `b > a`, `b` is strictly greater than `a`, so output `b`.
- Else (`a == b`), both numbers are equal, so output `"Both numbers are equal"`.

---

## 4. Algorithm/Steps
1. **Start**
2. Declare two 64-bit integer variables `a` and `b` of type `long long`.
3. Read the two integers from standard input (`cin >> a >> b`).
4. Check if `a > b`:
   - If true, print `a`.
5. Else if `b > a`:
   - If true, print `b`.
6. Else:
   - Print `"Both numbers are equal"`.
7. Exit the program with return code `0`.

---

## 5. Source Code

```cpp
#include <iostream>
using namespace std;

int main()
{
    long long a, b;
    cin >> a >> b;

    if (a > b)
        cout << a << endl;
    else if (b > a)
        cout << b << endl;
    else
        cout << "Both numbers are equal" << endl;

    return 0;
}
```
