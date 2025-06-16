# 100 Technical Aptitude Practice Questions (Basic Level) with Solutions

This file contains **100 basic-level practice questions** for Technical Aptitude, designed to develop foundational technical knowledge and problem-solving skills for fresher job aptitude tests, especially for AI/ML roles. Each question includes a description of the problem (e.g., programming fundamentals, data structures, algorithms, databases, networks, operating systems, AI/ML basics) and a detailed solution explaining the reasoning process. Topics cover basic syntax, control structures, arrays, simple algorithms, SQL queries, network protocols, process management, and introductory AI/ML concepts.

## Programming Fundamentals (1–20)

1. **Question**: What is the output of this C code: `int x = 5; printf("%d", x++);`?  
   **Solution**:  
   `x++` is post-increment, so `printf` uses the current value of `x` (5), then increments `x` to 6.  
   **Answer**: 5

2. **Question**: In Python, what is the output of: `print(3 * "hello")`?  
   **Solution**:  
   String repetition in Python multiplies the string: `3 * "hello"` produces `"hellohellohello"`.  
   **Answer**: hellohellohello

3. **Question**: What is the value of `x` after this Java code: `int x = 10; x += 5;`?  
   **Solution**:  
   `x += 5` is equivalent to `x = x + 5`. So, `x = 10 + 5 = 15`.  
   **Answer**: 15

4. **Question**: In C++, what is the output of: `int a = 3, b = 4; cout << a + b;`?  
   **Solution**:  
   `a + b = 3 + 4 = 7`. `cout` prints `7`.  
   **Answer**: 7

5. **Question**: What does this Python code do: `x = [1, 2, 3]; x.append(4)`?  
   **Solution**:  
   `append(4)` adds `4` to the end of the list `x`. New list: `[1, 2, 3, 4]`.  
   **Answer**: Adds 4 to the list

6. **Question**: In C, what is the output of: `int x = 8; printf("%d", x >> 1);`?  
   **Solution**:  
   `x >> 1` performs a right shift. `8` (binary `1000`) shifts to `0100` (4).  
   **Answer**: 4

7. **Question**: In Java, what is the output of: `boolean x = true; System.out.println(!x);`?  
   **Solution**:  
   `!x` negates `true` to `false`.  
   **Answer**: false

8. **Question**: What is the output of this Python code: `x = 10; y = 3; print(x // y)`?  
   **Solution**:  
   `//` is floor division: `10 // 3 = 3` (quotient without remainder).  
   **Answer**: 3

9. **Question**: In C++, what is the output of: `int x = 5; if(x > 3) cout << "Yes"; else cout << "No";`?  
   **Solution**:  
   `x = 5 > 3`, so `if` condition is true. Prints `Yes`.  
   **Answer**: Yes

10. **Question**: In Python, what is the output of: `for i in range(3): print(i)`?  
    **Solution**:  
    `range(3)` generates `0, 1, 2`. Loop prints each value.  
    **Answer**:  
    0  
    1  
    2

11. **Question**: In C, what is the output of: `int x = 3; printf("%d", x & 1);`?  
    **Solution**:  
    `x & 1` performs bitwise AND. `3` (binary `11`) AND `1` (binary `01`) = `01` (1).  
    **Answer**: 1

12. **Question**: In Java, what is the output of: `int x = 7; System.out.println(x % 2);`?  
    **Solution**:  
    `%` is modulus: `7 % 2 = 1` (remainder).  
    **Answer**: 1

13. **Question**: In Python, what is the output of: `x = [1, 2]; x.pop(0); print(x)`?  
    **Solution**:  
    `pop(0)` removes the element at index `0` (1). New list: `[2]`.  
    **Answer**: [2]

14. **Question**: In C++, what is the output of: `int x = 4; cout << ++x;`?  
    **Solution**:  
    `++x` is pre-increment, so `x` becomes `5`, and `5` is printed.  
    **Answer**: 5

15. **Question**: In C, what is the output of: `int x = 5; printf("%d", x | 2);`?  
    **Solution**:  
    `x | 2` performs bitwise OR. `5` (binary `101`) OR `2` (binary `010`) = `111` (7).  
    **Answer**: 7

16. **Question**: In Python, what is the output of: `x = {1, 2, 2}; print(len(x))`?  
    **Solution**:  
    Sets remove duplicates: `{1, 2, 2}` becomes `{1, 2}`. `len` returns `2`.  
    **Answer**: 2

17. **Question**: In Java, what is the output of: `String s = "Hello"; System.out.println(s.length());`?  
    **Solution**:  
    `length()` returns the number of characters in `"Hello"`, which is `5`.  
    **Answer**: 5

18. **Question**: In C++, what is the output of: `int x = 10; while(x > 8) { cout << x << " "; x--; }`?  
    **Solution**:  
    Loop runs while `x > 8`: prints `10`, then `9`.  
    **Answer**: 10 9

19. **Question**: In Python, what is the output of: `x = 5; print(x ** 2)`?  
    **Solution**:  
    `**` is exponentiation: `5 ** 2 = 25`.  
    **Answer**: 25

20. **Question**: In C, what is the output of: `int x = 6; printf("%d", x ^ 3);`?  
    **Solution**:  
    `x ^ 3` performs bitwise XOR. `6` (binary `110`) XOR `3` (binary `011`) = `101` (5).  
    **Answer**: 5

## Data Structures (21–40)

21. **Question**: What is the time complexity of accessing an element in an array?  
    **Solution**:  
    Arrays allow direct index-based access, which is constant time.  
    **Answer**: O(1)

22. **Question**: In a singly linked list, what is the time complexity to insert a node at the beginning?  
    **Solution**:  
    Inserting at the head updates the head pointer, which is constant time.  
    **Answer**: O(1)

23. **Question**: What is the output of this Python code for a stack: `s = []; s.append(1); s.append(2); s.pop(); print(s)`?  
    **Solution**:  
    Stack (LIFO): `append` adds `1`, `2`. `pop` removes `2`. Stack: `[1]`.  
    **Answer**: [1]

24. **Question**: In a queue, what is the order of elements after: enqueue(1), enqueue(2), dequeue(), enqueue(3)?  
    **Solution**:  
    Queue (FIFO): Enqueue `1`, `2`. Dequeue removes `1`. Enqueue `3`. Queue: `2, 3`.  
    **Answer**: 2, 3

25. **Question**: What is the time complexity of searching an element in an unsorted array of size n?  
    **Solution**:  
    Linear search checks each element, worst case n checks.  
    **Answer**: O(n)

26. **Question**: In a binary tree, what is the maximum number of nodes at level k (root at level 0)?  
    **Solution**:  
    At level k, maximum nodes = 2^k.  
    **Answer**: 2^k

27. **Question**: What is the output of this Python code for a list: `x = [1, 2, 3]; x.insert(1, 4); print(x)`?  
    **Solution**:  
    `insert(1, 4)` adds `4` at index `1`. New list: `[1, 4, 2, 3]`.  
    **Answer**: [1, 4, 2, 3]

28. **Question**: What is the time complexity of inserting an element at the end of a dynamic array (amortized)?  
    **Solution**:  
    Appending to a dynamic array is O(1) amortized, as resizing is rare.  
    **Answer**: O(1)

29. **Question**: In a circular queue with size 5, after enqueue(1, 2, 3), dequeue(), enqueue(4), what is the front element?  
    **Solution**:  
    Enqueue `1, 2, 3`. Dequeue removes `1`. Enqueue `4`. Front: `2`.  
    **Answer**: 2

30. **Question**: What is the height of a binary tree with 7 nodes in a balanced configuration?  
    **Solution**:  
    Balanced binary tree: height = ⌊log₂(7)⌋ = 2 (levels 0, 1, 2).  
    **Answer**: 2

31. **Question**: In Python, what is the output of: `d = {1: 'a', 2: 'b'}; print(d[1])`?  
    **Solution**:  
    Dictionary access by key: `d[1]` returns `'a'`.  
    **Answer**: a

32. **Question**: What is the time complexity of deleting the last node in a singly linked list with n nodes?  
    **Solution**:  
    Traverse to the second-to-last node to update the pointer: O(n).  
    **Answer**: O(n)

33. **Question**: In a stack, after push(1), push(2), pop(), push(3), what is the top element?  
    **Solution**:  
    Stack (LIFO): Push `1`, `2`. Pop removes `2`. Push `3`. Top: `3`.  
    **Answer**: 3

34. **Question**: What is the time complexity of searching in a binary search tree with n nodes (balanced)?  
    **Solution**:  
    Balanced BST search follows height, which is O(log n).  
    **Answer**: O(log n)

35. **Question**: In Python, what is the output of: `s = {1, 2, 3}; s.add(4); print(s)`?  
    **Solution**:  
    `add(4)` adds `4` to the set. New set: `{1, 2, 3, 4}`.  
    **Answer**: {1, 2, 3, 4}

36. **Question**: What is the space complexity of storing a binary tree with n nodes?  
    **Solution**:  
    Each node stores data and two pointers, total O(n) space.  
    **Answer**: O(n)

37. **Question**: In a queue, after enqueue(1, 2), dequeue(), enqueue(3, 4), dequeue(), what is the front element?  
    **Solution**:  
    Enqueue `1, 2`. Dequeue removes `1`. Enqueue `3, 4`. Dequeue removes `2`. Front: `3`.  
    **Answer**: 3

38. **Question**: What is the time complexity of inserting a key into a hash table (average case)?  
    **Solution**:  
    Average case with good hash function: O(1) for insertion.  
    **Answer**: O(1)

39. **Question**: In Python, what is the output of: `x = [1, 2, 3]; x.remove(2); print(x)`?  
    **Solution**:  
    `remove(2)` deletes the first occurrence of `2`. New list: `[1, 3]`.  
    **Answer**: [1, 3]

40. **Question**: What is the maximum number of nodes in a binary tree of height h?  
    **Solution**:  
    Maximum nodes = 2^(h+1) - 1 (sum of nodes from level 0 to h).  
    **Answer**: 2^(h+1) - 1

## Algorithms (41–60)

41. **Question**: What is the time complexity of bubble sort for n elements?  
    **Solution**:  
    Bubble sort compares and swaps in nested loops: O(n²).  
    **Answer**: O(n²)

42. **Question**: In Python, what is the output of this linear search: `x = [3, 1, 4]; print(x.index(4))`?  
    **Solution**:  
    `index(4)` returns the first index of `4`, which is `2`.  
    **Answer**: 2

43. **Question**: What is the time complexity of binary search on a sorted array of n elements?  
    **Solution**:  
    Binary search halves the search space each step: O(log n).  
    **Answer**: O(log n)

44. **Question**: What is the output of this C code for factorial: `int fact(int n) { if(n == 0) return 1; return n * fact(n-1); } printf("%d", fact(3));`?  
    **Solution**:  
    `fact(3)` = 3 × `fact(2)` = 3 × 2 × `fact(1)` = 3 × 2 × 1 = 6.  
    **Answer**: 6

45. **Question**: What is the space complexity of a recursive factorial algorithm?  
    **Solution**:  
    Recursive factorial uses O(n) stack space for n calls.  
    **Answer**: O(n)

46. **Question**: In Python, what is the output of: `x = [5, 2, 8]; print(sorted(x))`?  
    **Solution**:  
    `sorted(x)` returns a new sorted list: `[2, 5, 8]`.  
    **Answer**: [2, 5, 8]

47. **Question**: What is the time complexity of finding the maximum element in an unsorted array of n elements?  
    **Solution**:  
    Scan all elements: O(n).  
    **Answer**: O(n)

48. **Question**: In C, what is the output of this sum code: `int sum(int n) { if(n == 0) return 0; return n + sum(n-1); } printf("%d", sum(4));`?  
    **Solution**:  
    `sum(4)` = 4 + `sum(3)` = 4 + 3 + `sum(2)` = 4 + 3 + 2 + `sum(1)` = 4 + 3 + 2 + 1 = 10.  
    **Answer**: 10

49. **Question**: What is the time complexity of selection sort for n elements?  
    **Solution**:  
    Selection sort finds the minimum in each pass: O(n²).  
    **Answer**: O(n²)

50. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(x[::-1])`?  
    **Solution**:  
    Slicing `[::-1]` reverses the list: `[3, 2, 1]`.  
    **Answer**: [3, 2, 1]

51. **Question**: What is the time complexity of checking if an element exists in a sorted array using binary search?  
    **Solution**:  
    Binary search: O(log n).  
    **Answer**: O(log n)

52. **Question**: In C++, what is the output of: `int x = 5; for(int i = 1; i <= 3; i++) x += i; cout << x;`?  
    **Solution**:  
    Loop: `x = 5 + 1 + 2 + 3 = 11`.  
    **Answer**: 11

53. **Question**: What is the space complexity of bubble sort?  
    **Solution**:  
    Bubble sort uses a constant amount of extra space: O(1).  
    **Answer**: O(1)

54. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(sum(x))`?  
    **Solution**:  
    `sum(x)` adds elements: `1 + 2 + 3 = 6`.  
    **Answer**: 6

55. **Question**: What is the time complexity of inserting an element into a sorted array of n elements?  
    **Solution**:  
    Shift elements to make space: O(n).  
    **Answer**: O(n)

56. **Question**: In C, what is the output of: `int a = 3, b = 5; if(a > b) printf("%d", a); else printf("%d", b);`?  
    **Solution**:  
    `3 > 5` is false, so print `b = 5`.  
    **Answer**: 5

57. **Question**: What is the time complexity of merging two sorted arrays of sizes m and n?  
    **Solution**:  
    Merge process compares and copies: O(m + n).  
    **Answer**: O(m + n)

58. **Question**: In Python, what is the output of: `x = "abc"; print(x.upper())`?  
    **Solution**:  
    `upper()` converts to uppercase: `"ABC"`.  
    **Answer**: ABC

59. **Question**: What is the time complexity of reversing an array of n elements?  
    **Solution**:  
    Swap elements from ends to middle: O(n).  
    **Answer**: O(n)

60. **Question**: In C++, what is the output of: `int x = 4; x *= 3; cout << x;`?  
    **Solution**:  
    `x *= 3` means `x = x * 3 = 4 * 3 = 12`.  
    **Answer**: 12

## Database Basics (61–70)

61. **Question**: What does the SQL query `SELECT * FROM table_name;` do?  
    **Solution**:  
    Retrieves all columns and rows from `table_name`.  
    **Answer**: Fetches all data

62. **Question**: What is the output of: `SELECT name FROM employees WHERE salary > 50000;`?  
    **Solution**:  
    Returns the `name` column for rows where `salary` exceeds 50000.  
    **Answer**: Names of employees with salary > 50000

63. **Question**: What does the SQL keyword `PRIMARY KEY` ensure?  
    **Solution**:  
    Ensures each value in the column is unique and not null.  
    **Answer**: Uniqueness and non-null

64. **Question**: What is the result of: `SELECT COUNT(*) FROM students WHERE age = 20;`?  
    **Solution**:  
    Counts the number of rows where `age` is 20.  
    **Answer**: Number of students aged 20

65. **Question**: What does `DELETE FROM table_name WHERE id = 1;` do?  
    **Solution**:  
    Removes the row where `id` equals 1.  
    **Answer**: Deletes row with id = 1

66. **Question**: What is the purpose of the SQL `JOIN` clause?  
    **Solution**:  
    Combines rows from two or more tables based on a related column.  
    **Answer**: Merges tables

67. **Question**: What does `INSERT INTO users (name, age) VALUES ('Alice', 25);` do?  
    **Solution**:  
    Adds a new row to `users` with `name = 'Alice'` and `age = 25`.  
    **Answer**: Inserts a new user

68. **Question**: What is the output of: `SELECT MAX(salary) FROM employees;`?  
    **Solution**:  
    Returns the highest value in the `salary` column.  
    **Answer**: Maximum salary

69. **Question**: What does the SQL `WHERE` clause do?  
    **Solution**:  
    Filters rows based on a specified condition.  
    **Answer**: Filters data

70. **Question**: What is the result of: `UPDATE products SET price = 100 WHERE id = 5;`?  
    **Solution**:  
    Sets `price` to 100 for the row where `id` is 5.  
    **Answer**: Updates price for id = 5

## Computer Networks (71–80)

71. **Question**: What is the purpose of the IP address?  
    **Solution**:  
    Uniquely identifies a device on a network.  
    **Answer**: Device identification

72. **Question**: What is the port number used by HTTP?  
    **Solution**:  
    HTTP uses port 80 for communication.  
    **Answer**: 80

73. **Question**: What does the acronym TCP stand for?  
    **Solution**:  
    Transmission Control Protocol, ensures reliable data transfer.  
    **Answer**: Transmission Control Protocol

74. **Question**: What is the role of DNS in networking?  
    **Solution**:  
    Translates domain names (e.g., google.com) to IP addresses.  
    **Answer**: Domain name resolution

75. **Question**: What is the difference between IPv4 and IPv6?  
    **Solution**:  
    IPv4 uses 32-bit addresses (e.g., 192.168.0.1); IPv6 uses 128-bit addresses for more capacity.  
    **Answer**: Address length and capacity

76. **Question**: What does the term "bandwidth" refer to?  
    **Solution**:  
    Maximum data transfer rate of a network connection.  
    **Answer**: Data transfer rate

77. **Question**: What is the purpose of a router in a network?  
    **Solution**:  
    Forwards data packets between networks.  
    **Answer**: Routes data

78. **Question**: What is the default subnet mask for a Class C IP address?  
    **Solution**:  
    Class C uses 24 bits for the network: 255.255.255.0.  
    **Answer**: 255.255.255.0

79. **Question**: What is the function of the ARP protocol?  
    **Solution**:  
    Maps IP addresses to MAC addresses.  
    **Answer**: Address resolution

80. **Question**: What does UDP stand for, and how does it differ from TCP?  
    **Solution**:  
    User Datagram Protocol; UDP is faster but less reliable than TCP (no error checking).  
    **Answer**: User Datagram Protocol, less reliable

## Operating Systems (81–90)

81. **Question**: What is the role of an operating system?  
    **Solution**:  
    Manages hardware, software, and provides user interface.  
    **Answer**: Resource management

82. **Question**: What is a process in an operating system?  
    **Solution**:  
    A program in execution, with its own memory and resources.  
    **Answer**: Executing program

83. **Question**: What is the purpose of a scheduler in an OS?  
    **Solution**:  
    Allocates CPU time to processes for efficient execution.  
    **Answer**: CPU allocation

84. **Question**: What is a deadlock in an operating system?  
    **Solution**:  
    A situation where processes hold resources and wait for others, causing a standstill.  
    **Answer**: Resource conflict standstill

85. **Question**: What does the term "virtual memory" refer to?  
    **Solution**:  
    Uses disk space to extend RAM, allowing larger programs to run.  
    **Answer**: Extended memory

86. **Question**: What is the function of a file system in an OS?  
    **Solution**:  
    Organizes and manages data storage on disks.  
    **Answer**: Data organization

87. **Question**: What is a thread in an operating system?  
    **Solution**:  
    A lightweight process sharing the same memory space as its parent process.  
    **Answer**: Lightweight process

88. **Question**: What is the purpose of an interrupt in an OS?  
    **Solution**:  
    Signals the CPU to handle an urgent event (e.g., hardware input).  
    **Answer**: Event handling

89. **Question**: What is the difference between a kernel and a shell?  
    **Solution**:  
    Kernel manages system resources; shell is the user interface to interact with the OS.  
    **Answer**: Kernel: core, Shell: interface

90. **Question**: What is the role of a page table in virtual memory?  
    **Solution**:  
    Maps virtual addresses to physical addresses.  
    **Answer**: Address mapping

## AI/ML Foundations (91–100)

91. **Question**: What is supervised learning in machine learning?  
    **Solution**:  
    Model trains on labeled data (input-output pairs) to predict outputs.  
    **Answer**: Learning with labeled data

92. **Question**: What is the purpose of a loss function in ML?  
    **Solution**:  
    Measures the error between predicted and actual outputs to guide optimization.  
    **Answer**: Error measurement

93. **Question**: What is overfitting in machine learning?  
    **Solution**:  
    Model learns training data too well, including noise, and performs poorly on new data.  
    **Answer**: Excessive training fit

94. **Question**: What is the role of a feature in ML?  
    **Solution**:  
    An input variable used to make predictions.  
    **Answer**: Input variable

95. **Question**: What is the purpose of splitting data into training and testing sets?  
    **Solution**:  
    Training set trains the model; testing set evaluates its performance on unseen data.  
    **Answer**: Model training and evaluation

96. **Question**: What is a neuron in a neural network?  
    **Solution**:  
    A computational unit that processes inputs, applies weights, and produces an output.  
    **Answer**: Computational unit

97. **Question**: What is the activation function in a neural network?  
    **Solution**:  
    Introduces non-linearity to decide whether a neuron should activate.  
    **Answer**: Non-linearity function

98. **Question**: What is gradient descent in ML?  
    **Solution**:  
    Optimization algorithm to minimize the loss function by adjusting model parameters.  
    **Answer**: Parameter optimization

99. **Question**: What is unsupervised learning in ML?  
    **Solution**:  
    Model finds patterns in unlabeled data without predefined outputs.  
    **Answer**: Learning without labels

100. **Question**: What is the purpose of normalization in ML?  
    **Solution**:  
    Scales features to a standard range to improve model performance.  
    **Answer**: Feature scaling