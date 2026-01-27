# python-basic-challenges


1. Ek variable `x` banao aur usme 10 store karo. Phir usko print karo. (Output: 10)  
2. Do variables `a=5`, `b=3` banao. Unka sum print karo. (Output: 8)  
3. Ek string variable `name` mein "El" store karo aur print karo. (Output: El)  
4. Ek float `pi` mein 3.14 daalo aur print karo. (Output: 3.14)  
5. Do numbers `p=10`, `q=20` compare karo agar p < q hai to "Yes" print karo. (Output: Yes)  
6. Ek boolean `is_even = (4 % 2 == 0)` banao aur print karo. (Output: True)  
7. `x=7`, `y=2` se x // y (floor division) print karo. (Output: 3)  
8. `a= True`, `b= False` se a and b print karo. (Output: False)  
9. Ek variable `age=25` banao, agar age >=18 to "Adult" print karo warna "Minor". (Output: Adult)  
10. `num= -5` ka absolute value print karo (abs() use karo). (Output: 5)  
11. Do strings "Hello" aur "World" ko concatenate karke print karo. (Output: HelloWorld)  
12. `x=10` ko x += 5 karke print karo. (Output: 15)  
13. `a=4`, `b=5` se a ** b (power) print karo. (Output: 1024)  
14. Ek variable `temp=37.5` banao, usko int mein convert karke print karo. (Output: 37)  
15. `n=9` agar n % 3 ==0 and n % 2 !=0 to "Special" print karo. (Test: Yes for 9)  
16. Do variables swap karo without extra variable: a=1, b=2 → a=2, b=1 print.  
17. `x= "123"` ko int mein convert kar print karo. (Output: 123)  
18. `is_raining=True`, `is_cold=False` se not (is_raining or is_cold) print karo. (Output: False)  
19. Ek variable `score=85` banao, agar 80 <= score <90 to "B Grade" print.  
20. `a=10/3` print karo with 2 decimal places (format use). (Output: 3.33)

### 2. Loops & Control Flow (20 Challenges)
Focus: for, while, if-elif-else, break, continue, range().

21. 1 se 10 tak numbers print karo using for loop. (Output: 1 2 ...10)  
22. Ek while loop se 5 se 0 tak countdown print karo. (Output: 5 4 3 2 1 0)  
23. 1 se 20 tak even numbers print karo using if in loop. (2 4 ...20)  
24. User se input leke (int) agar positive to "Positive", negative "Negative", zero "Zero".  
25. For loop se 1 se 5 tak ka sum calculate kar print (15)  
26. While loop mein break use karke jab i=5 ho to loop stop, i=1 to 10.  
27. 1 se 10 tak odd numbers skip karo using continue in for loop. (2 4 6 8 10)  
28. Nested if: age=20, gender="M" agar age>18 and gender=="M" to "Adult Male".  
29. FizzBuzz basic: 1-10 mein 3 ka multiple "Fizz", 5 "Buzz", both "FizzBuzz".  
30. While loop se user input lete raho jab tak "quit" na type kare.  
31. For i in range(10): agar i>5 to print i*2. (12 14 16 18)  
32. 1 se n tak sum (n= input) using loop. (Test n=5:15)  
33. Reverse loop: 10 se 1 tak print using range(10,0,-1).  
34. If-elif ladder: marks=75 → A(90+), B(70-89), C(50-69), Fail(<50). (B)  
35. Infinite while loop banao lekin break se 3 baar loop kar ke exit.  
36. For loop se string "Python" ke har char print karo vertically. (P y t h o n)  
37. 1 se 100 tak primes print karo (simple loop with if).  
38. Nested loop: 3x3 grid print (1 2 3 \n 4 5 6 \n 7 8 9)  
39. User input number ka factorial using while (5:120)  
40. Switch jaise if-elif: day=1 "Monday", 2 "Tuesday" ... else "Invalid".

### 3. Functions & Modules (20 Challenges)
Focus: def, return, parameters, import math/random/os, etc.

41. Ek function `add(a,b)` banao jo sum return kare. Call: add(3,4) →7  
42. Function `is_even(n)` return True if even. (Test: is_even(4) True)  
43. Default param: def greet(name="El") → "Hello El"  
44. Import math: function mein math.sqrt(16) use kar print 4.0  
45. Function `max_of_three(a,b,c)` return max without max().  
46. Import random: function random number 1-10 generate kare.  
47. Lambda function: double = lambda x: x*2 → double(5)=10  
48. Function factorial(n) recursive banao. (5:120)  
49. Import os: function current directory print kare (os.getcwd())  
50. Function multiple returns: def div_mod(a,b) return a//b, a%b  
51. Global variable: function mein global x=10 change to 20.  
52. Import re: function string mein email validate (simple re.match)  
53. Function list ko sort kare without sorted() (bubble sort simple).  
54. Anonymous function filter even numbers from list.  
55. Import sys: function sys.argv se command line args print.  
56. Function *args use: sum_all(*args) sum of all args.  
57. Function **kwargs: print_person(name="El", age=25) → details print.  
58. Docstring wala function: def hello() """This is doc""" print hello.__doc__  
59. Import datetime: function current date print.  
60. Function decorator simple: def deco(func) wrap with print "Start" "End".

### 4. Lists (20 Challenges)
Focus: Create, append, index, slice, comprehension, sort, etc.

61. Empty list banao, 1,2,3 append kar print. ([1,2,3])  
62. List [1,2,3,4] ka index 2 ka value print (3)  
63. Slice: lst=[0,1,2,3,4] lst[1:4] print ([1,2,3])  
64. List comprehension: [x**2 for x in range(5)] ([0,1,4,9,16])  
65. List sort: [3,1,4,2] sorted print [1,2,3,4]  
66. Remove duplicate: [1,2,2,3] → [1,2,3] (use list(set()))  
67. List reverse: [1,2,3] → [3,2,1] (reverse() or [::-1])  
68. Find max in list without max() (loop use).  
69. Two lists merge: a=[1,2], b=[3,4] → [1,2,3,4]  
70. List mein even numbers filter (comprehension). ([2,4,6] from [1-6])  
71. Nested list: [[1,2],[3,4]] ka element [1][0]=3 print.  
72. List pop last element: [1,2,3] → pop()=3, list=[1,2]  
73. Insert at position: lst=[1,3] insert 2 at index 1 → [1,2,3]  
74. Count occurrence: [1,2,1,1] mein 1 ka count=3  
75. List to string: ['H','e','l','l','o'] → "Hello" (join)  
76. Zip two lists: names=["El","Alex"], ages=[25,30] → [('El',25),('Alex',30)]  
77. Enumerate: for i,v in enumerate(['a','b']) print i v (0 a,1 b)  
78. List comprehension if: [x for x in range(10) if x%2==0] ([0,2,4,6,8])  
79. Flatten nested list: [[1,2],[3]] → [1,2,3] (loop or comp)  
80. List rotate left: [1,2,3,4] → [2,3,4,1]

### 5. Dictionaries (20 Challenges)
Focus: Create, key-value, get, items, update, etc.

81. Empty dict, 'name':'El' add kar print. ({'name':'El'})  
82. Dict {'a':1,'b':2} ka 'b' value print (2)  
83. Keys list: d={'x':10,'y':20} list(d.keys())=['x','y']  
84. Update dict: d1={'a':1}, d2={'b':2} → merge to {'a':1,'b':2}  
85. Dict comprehension: {x:x**2 for x in range(3)} ({0:0,1:1,2:4})  
86. Check key exists: 'name' in {'name':'El'} → True  
87. Delete key: del d['key']  
88. Sorted dict by keys: {'b':2,'a':1} → {'a':1,'b':2} (sorted(dict))  
89. Get value with default: d.get('age',0) →0 if not exist  
90. Loop dict: for k,v in d.items() print k v  
91. Nested dict: {'person':{'name':'El','age':25}} ka age print.  
92. Dict from two lists: keys=['a','b'], vals=[1,2] → {'a':1,'b':2} (zip)  
93. Count chars in string: "hello" → {'h':1,'e':1,'l':2,'o':1}  
94. Max value key: {'a':10,'b':20} → 'b'  
95. Dict copy: d.copy()  
96. Clear dict: d.clear() → {}  
97. Dict values sum: {'a':1,'b':2} →3 (sum(d.values()))  
98. Invert dict: {'a':1,'b':2} → {1:'a',2:'b'} (assume unique vals)  
99. Dict filter: keep only even values {'a':1,'b':2,'c':3} → {'b':2}  
100. Merge multiple dicts: dict1, dict2, dict3 into one.

### 6. Sets (15 Challenges)  // Extra for strength
Focus: Unique, add, union, intersection, difference.

101. Empty set, 1,2,3 add kar print ({1,2,3})  
102. Set [1,2,2,3] se duplicates remove → {1,2,3}  
103. Union: {1,2} | {2,3} → {1,2,3}  
104. Intersection: {1,2,3} & {2,3,4} → {2,3}  
105. Difference: {1,2,3} - {2} → {1,3}  
106. Check subset: {1,2} issubset {1,2,3} → True  
107. Add element: s.add(4)  
108. Remove: s.remove(2) (error if not exist)  
109. Discard: s.discard(5) (no error)  
110. Pop random: s.pop()  
111. Symmetric difference: {1,2} ^ {2,3} → {1,3}  
112. Frozen set: frozenset([1,2]) (immutable)  
113. Set comprehension: {x**2 for x in range(3)} ({0,1,4})  
114. Count unique in list: len(set([1,2,1]))=2  
115. Check membership: 1 in {1,2} → True  

