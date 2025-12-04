

##  What is Time Complexity?
Time Complexity = Code ko input size **n** badhne par kitna time lagta hai.

- n = array size  
- n = database rows  
- n = loop iterations  
- n = API request count  

Time complexity **code ki speed** ko measure karta hai, not actual seconds.

---

## 🚀 Examples

### **1. Single Loop (O(n))**
```php
for ($i = 0; $i < n; $i++) {
    print($i);
}

Time Complexity → O(n)
(Linear — input jitna bada, time utna bada)


---

2. Nested Loop (O(n²))

for (let i = 0; i < n; i++) {
    for (let j = 0; j < n; j++) {
        console.log("*");
    }
}

Time Complexity → O(n²)
(Each loop runs n times → n × n)


---

⭐ Types of Time Complexity

1. Best Case


2. Average Case


3. Worst Case ← (Most Important)




---

📘 Example: Finding Grade

if marks < 30:
    print("D")
elif marks <= 50:
    print("C")
elif marks <= 70:
    print("B")
elif marks >= 90:
    print("A")

Find grade of 25

Condition first line me match ho jata hai
✔ Best Case


Find grade of 95

Puri conditions check karni padti hain
✔ Worst Case


> We always calculate time complexity using the Worst Case.




---

⚠ Important Rules (Must Remember)

1️⃣ Time Taken ≠ Time Complexity

Even if code takes 1 sec or 10 sec → Complexity does not change.

2️⃣ Time Complexity depends ONLY on input size

Laptop speed, internet, mobile speed does NOT matter.

3️⃣ Constants ko ignore karte hain

O(2n), O(5n) → O(n)
O(n² + n) → O(n²)

4️⃣ Worst Case pe complexity calculate hoti hai


---

🧩 More Practical Coding Examples

✔ Separate Loops → O(n)

for (let i = 0; i < n; i++) {}   // O(n)
for (let j = 0; j < n; j++) {}   // O(n)

Total = n + n = 2n → O(n)


---

✔ Double Nested Loops → O(n²)

for (let i = 0; i < n; i++) {
  for (let j = 0; j < n; j++) {}
}


---

✔ Triple Nested Loop → O(n³)

for (i = 0; i < n; i++) {
  for (j = 0; j < n; j++) {
    for (k = 0; k < n; k++) {}
  }
}


---

🧮 SPACE COMPLEXITY

Space Complexity = Program ko chalne ke liye extra memory kitni lagti hai.

✔ O(1) Space

(Only 1 variable)

let x = 10;

✔ O(n) Space

(Uses extra memory for array)

let arr = [1,2,3,4,5];


---

📌 Summary Table

Code Pattern	Time Complexity

Single Loop	O(n)
Two separate loops	O(n)
Nested 2 loops	O(n²)
Nested 3 loops	O(n³)
Binary Search	O(log n)
Sorting (Quick/Heap/Merge)	O(n log n)
HashMap lookup	O(1)



---

⭐ Super Important Lines (Lifelong Useful)

Time complexity real-time nahi hota, growth hota hai.

Worst-case hi consider hota hai.

Constants ignore hote hain.

Nested loops → multiply.

Separate loops → add = still O(n).

Space complexity → extra memory used.



---

---

If you want, I can also give you a **second version with Laravel, Django, SQL relatable examples** to add below this.