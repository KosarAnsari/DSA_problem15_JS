# 🚀 Day 15 of 21-Day DSA Challenge – Selection Sort

## 📌 Topic: Selection Sort in JavaScript

### 📖 Description:
Selection Sort is a simple and intuitive sorting algorithm. It works by **repeatedly finding the minimum element** (considering ascending order) from the unsorted part and putting it at the beginning.

### 🔍 How It Works:
1. Iterate over the array.
2. For each index, find the smallest element in the unsorted portion.
3. Swap it with the current index.
4. Repeat until the array is fully sorted.

### 📦 Code:
```js
function selSort(array) {
    for (let i = 0; i < array.length; i++) {
        let min = i;
        for (let j = i + 1; j < array.length; j++) {
            if (array[j] < array[min]) {
                min = j;
            }
        }
        if (i !== min) {
            let temp = array[i];
            array[i] = array[min];
            array[min] = temp;
        }
    }
    return array;
}

let res = selSort([0, 2, 34, 22, 10, 19]);
console.log(res);  // Output: [0, 2, 10, 19, 22, 34]

🧠 What I Learned:

The concept of in-place sorting

Nested loops and element comparisons

How to perform element swapping using a temporary variable

Time complexity: O(n²)


📊 Output:

[0, 2, 10, 19, 22, 34]


---

📅 Challenge Progress:

✔️ Completed: Day 15/21
📚 Upcoming: More sorting and search techniques


---

🔗 Connect:

Let's connect on LinkedIn and share learning progress!

#JavaScript #DSA #21DaysChallenge #SelectionSort #SortingAlgorithms #CodeNewbie #FrontendDevelopment

