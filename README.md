# 🤝 Handshake Problem (Recursion + Complexity Analysis)

This repository demonstrates the classic **Handshake Problem** using a **recursive approach**, along with a detailed analysis of **time complexity, space complexity, and growth rate**.

---

## 📌 Problem Statement

If there are **n people** in a room and each pair shakes hands exactly once, how many total handshakes occur?

---

## 🧮 Mathematical Formula

The total number of handshakes is:

```math
H(n) = \frac{n(n-1)}{2}

```

This represents the number of unique pairs that can be formed from `n` people.

---

## 💻 Implementation (Recursive Approach)

```cpp
#include <iostream>
using namespace std;

int handshake(int n)
{
    if (n == 0 || n == 1)
        return 0;

    cout << n << endl;

    return handshake(n - 1) + (n - 1);
}
```

---

## 🔍 How It Works

The recursive relation:

```math

H(n) = H(n-1) + (n-1)

```

* First compute handshakes among `n-1` people
* Then add `(n-1)` new handshakes for the nth person

---

## ⏱️ Time Complexity

### Recurrence:

```math

T(n) = T(n-1) + O(1)

```

### Result:

```math

Time Complexity = Θ(n)


```

---

## 📦 Space Complexity

### Breakdown:

* **Input Space** = Θ(1) (only integer `n`)
* **Auxiliary Space** = Θ(n) (due to recursion stack)

### Final:

```math

Space Complexity = Θ(n)

```
---

## 📈 Growth Rate of Output

```math

H(n) = \frac{n(n-1)}{2} \approx Θ(n^2)

```

✔ Output grows **quadratically**
✔ Algorithm runs in **linear time**

---

## ⚠️ Important Concept

> **Time Complexity ≠ Growth of Output**

| Concept         | Meaning                       |
| --------------- | ----------------------------- |
| Time Complexity | How fast the algorithm runs   |
| Growth Rate     | How fast the result increases |

---

## 🔁 Alternative Approaches

### 1. Iterative Solution

```cpp
int handshake(int n) {
    int sum = 0;
    for(int i = 1; i < n; i++)
        sum += i;
    return sum;
}
```

* Time: Θ(n)
* Space: Θ(1)

---

### 2. Direct Formula (Optimal)

```cpp
int handshake(int n) {
    return (n * (n - 1)) / 2;
}
```

* Time: Θ(1)
* Space: Θ(1)

---

## 🧠 Key Learnings

* Recursive problems often hide **mathematical patterns**
* Space complexity in recursion depends on **call stack depth**
* Always distinguish:

  * Algorithm efficiency
  * Output growth

---

## 📚 Topics Covered

* Recursion
* Recurrence Relations
* Time Complexity Analysis
* Space Complexity Analysis
* Growth Rate (Asymptotic Analysis)

---

## 🚀 Future Improvements

* Add recursion tree visualization
* Compare iterative vs recursive performance
* Extend to combinatorics problems

---

## 📌 Author

**[Avinandan Bose](https://github.com/AvinandanBose)**

---

## 📝 License

This project is open-source and available under the [MIT License](https://www.google.com/search?q=LICENSE).

## ⭐ If you found this useful

Give this repo a ⭐ and explore more algorithmic insights!




<br>
<br>
<br>

<h2></h2>
<h2> 👉 <a href="https://github.com/AvinandanBose/CPLUSPLUS_DataStructure"> 𝑪++ 𝑷𝒓𝒐𝒈𝒓𝒂𝒎  𝒐𝒏 𝑯𝒂𝒏𝒅 𝑺𝒉𝒂𝒌𝒆 𝑷𝒓𝒐𝒃𝒍𝒆𝒎 </h2>


