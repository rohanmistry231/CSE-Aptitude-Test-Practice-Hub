# 100 Technical Aptitude Practice Questions (Intermediate Level) with Solutions

This file contains **100 intermediate-level practice questions** for Technical Aptitude, designed to enhance technical knowledge and problem-solving skills for fresher job aptitude tests, especially for AI/ML roles. Each question includes a detailed description of the problem (e.g., programming, data structures, algorithms, databases, networks, operating systems, AI/ML) and a comprehensive solution explaining the reasoning process. Topics cover moderately complex programming logic, linked lists, trees, sorting algorithms, SQL joins, network layers, process synchronization, and AI/ML model evaluation.

## Programming Fundamentals (1–20)

1. **Question**: What is the output of this C code: `int x = 5; printf("%d %d", x++, ++x);`?  
   **Solution**:  
   In `printf`, arguments are evaluated right-to-left. `++x` increments `x` to 6, then `x++` uses 6 and increments `x` to 7. Output: `6 6`.  
   **Answer**: 6 6

2. **Question**: In Python, what is the output of: `x = [1, 2, 3]; y = x; y[0] = 4; print(x)`?  
   **Solution**:  
   `y = x` creates a reference to the same list. Modifying `y[0]` changes `x`. Output: `[4, 2, 3]`.  
   **Answer**: [4, 2, 3]

3. **Question**: In Java, what is the output of: `String s = "hello"; s = s.concat(" world"); System.out.println(s);`?  
   **Solution**:  
   `concat` creates a new string `"hello world"`. Output: `hello world`.  
   **Answer**: hello world

4. **Question**: In C++, what is the output of: `int x = 10; cout << (x > 5 ? x : 5);`?  
   **Solution**:  
   Ternary operator: `x > 5` is true, so prints `x = 10`.  
   **Answer**: 10

5. **Question**: In Python, what is the output of: `def f(x): x += 1; x = 5; f(x); print(x)`?  
   **Solution**:  
   Python passes integers by value. `x` inside `f` is local. Output: `5`.  
   **Answer**: 5

6. **Question**: In C, what is the output of: `int x = 10; printf("%d", x << 2);`?  
   **Solution**:  
   `x << 2` left-shifts `10` (binary `1010`) to `101000` (40).  
   **Answer**: 40

7. **Question**: In Java, what is the output of: `int[] arr = {1, 2, 3}; System.out.println(arr[arr.length - 1]);`?  
   **Solution**:  
   `arr.length - 1 = 2`. `arr[2] = 3`.  
   **Answer**: 3

8. **Question**: In Python, what is the output of: `x = {1: 'a', 2: 'b'}; x.update({2: 'c'}); print(x)`?  
   **Solution**:  
   `update` modifies key `2` to `'c'`. Output: `{1: 'a', 2: 'c'}`.  
   **Answer**: {1: 'a', 2: 'c'}

9. **Question**: In C++, what is the output of: `int x = 5; for(int i = 0; i < 3; i++) x *= 2; cout << x;`?  
   **Solution**:  
   Loop: `x = 5 * 2 * 2 * 2 = 40`.  
   **Answer**: 40

10. **Question**: In C, what is the output of: `int a = 7, b = 3; printf("%d", a ^ b);`?  
    **Solution**:  
    `a ^ b`: `7` (binary `111`) XOR `3` (binary `011`) = `100` (4).  
    **Answer**: 4

11. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(x[1:3])`?  
    **Solution**:  
    Slicing `[1:3]` includes indices 1 to 2: `[2, 3]`.  
    **Answer**: [2, 3]

12. **Question**: In Java, what is the output of: `int x = 15; System.out.println(x & (x - 1));`?  
    **Solution**:  
    `x & (x - 1)` clears the least significant set bit. `15` (binary `1111`) & `14` (binary `1110`) = `1110` (14).  
    **Answer**: 14

13. **Question**: In C++, what is the output of: `string s = "abc"; reverse(s.begin(), s.end()); cout << s;`?  
    **Solution**:  
    `reverse` reverses the string: `"abc"` becomes `"cba"`.  
    **Answer**: cba

14. **Question**: In Python, what is the output of: `x = lambda a: a * 2; print(x(3))`?  
    **Solution**:  
    Lambda function doubles input: `3 * 2 = 6`.  
    **Answer**: 6

15. **Question**: In C, what is the output of: `int x = 5; printf("%d", ~x);`?  
    **Solution**:  
    `~x` inverts bits of `5` (binary `00000101`) to `11111010` (two’s complement, -6).  
    **Answer**: -6

16. **Question**: In Java, what is the output of: `int x = 8; System.out.println(x >> 1);`?  
    **Solution**:  
    `x >> 1` right-shifts `8` (binary `1000`) to `0100` (4).  
    **Answer**: 4

17. **Question**: In Python, what is the output of: `x = [1, 2]; y = x.copy(); y[0] = 3; print(x)`?  
    **Solution**:  
    `copy()` creates a shallow copy. Modifying `y` doesn’t affect `x`. Output: `[1, 2]`.  
    **Answer**: [1, 2]

18. **Question**: In C++, what is the output of: `int x = 3; cout << (x << 1) + (x >> 1);`?  
    **Solution**:  
    `x << 1 = 3 * 2 = 6`. `x >> 1 = 3 / 2 = 1`. `6 + 1 = 7`.  
    **Answer**: 7

19. **Question**: In C, what is the output of: `int arr[3] = {1, 2, 3}; printf("%d", *(arr + 1));`?  
    **Solution**:  
    `*(arr + 1)` accesses `arr[1] = 2`.  
    **Answer**: 2

20. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(list(map(lambda x: x**2, x)))`?  
    **Solution**:  
    `map` applies square function: `[1², 2², 3²] = [1, 4, 9]`.  
    **Answer**: [1, 4, 9]

## Data Structures (21–40)

21. **Question**: What is the time complexity of inserting a node at the end of a singly linked list with n nodes?  
    **Solution**:  
    Traverse to the end to update the pointer: O(n).  
    **Answer**: O(n)

22. **Question**: In Python, what is the output of this stack operation: `s = []; s.append(1); s.append(2); s.append(3); s.pop(); s.pop(); print(s)`?  
    **Solution**:  
    Stack (LIFO): Push `1, 2, 3`. Pop removes `3`, then `2`. Stack: `[1]`.  
    **Answer**: [1]

23. **Question**: In a doubly linked list, what is the time complexity to delete a node given its pointer?  
    **Solution**:  
    Update prev/next pointers of adjacent nodes: O(1).  
    **Answer**: O(1)

24. **Question**: In a queue, after enqueue(1, 2, 3), dequeue(), enqueue(4), dequeue(), what is the front element?  
    **Solution**:  
    Queue (FIFO): Enqueue `1, 2, 3`. Dequeue removes `1`. Enqueue `4`. Dequeue removes `2`. Front: `3`.  
    **Answer**: 3

25. **Question**: What is the time complexity of searching in an unbalanced binary search tree with n nodes?  
    **Solution**:  
    Worst case (skewed tree) resembles a linked list: O(n).  
    **Answer**: O(n)

26. **Question**: In Python, what is the output of: `from collections import deque; q = deque([1, 2]); q.append(3); q.popleft(); print(q)`?  
    **Solution**:  
    Deque: Append `3`, popleft removes `1`. Deque: `[2, 3]`.  
    **Answer**: deque([2, 3])

27. **Question**: What is the time complexity of inserting an element in a min-heap with n elements?  
    **Solution**:  
    Insert at bottom, bubble up to restore heap property: O(log n).  
    **Answer**: O(log n)

28. **Question**: In a binary tree, what is the time complexity of finding the height?  
    **Solution**:  
    Recursively visit all nodes: O(n).  
    **Answer**: O(n)

29. **Question**: In Python, what is the output of: `d = {'a': 1, 'b': 2}; d.pop('a'); print(d)`?  
    **Solution**:  
    `pop('a')` removes key `'a'`. Output: `{'b': 2}`.  
    **Answer**: {'b': 2}

30. **Question**: What is the time complexity of deleting the root of a max-heap with n elements?  
    **Solution**:  
    Replace root with last element, bubble down: O(log n).  
    **Answer**: O(log n)

31. **Question**: In a circular linked list, what is the time complexity to insert a node after a given node?  
    **Solution**:  
    Update pointers of given and next node: O(1).  
    **Answer**: O(1)

32. **Question**: In Python, what is the output of: `s = {1, 2, 3}; s.discard(2); print(s)`?  
    **Solution**:  
    `discard(2)` removes `2`. Output: `{1, 3}`.  
    **Answer**: {1, 3}

33. **Question**: In a binary search tree, what is the time complexity to find the minimum element?  
    **Solution**:  
    Traverse to the leftmost node: O(h), where h is height (O(log n) if balanced).  
    **Answer**: O(log n) (balanced)

34. **Question**: What is the space complexity of a depth-first search (DFS) on a binary tree with n nodes?  
    **Solution**:  
    Recursion stack uses O(h), where h is height (O(log n) if balanced).  
    **Answer**: O(log n) (balanced)

35. **Question**: In Python, what is the output of: `x = [[1, 2], [3, 4]]; x[0].append(5); print(x)`?  
    **Solution**:  
    Append `5` to `x[0]`. Output: `[[1, 2, 5], [3, 4]]`.  
    **Answer**: [[1, 2, 5], [3, 4]]

36. **Question**: What is the time complexity of level-order traversal (BFS) of a binary tree with n nodes?  
    **Solution**:  
    Visit all nodes using a queue: O(n).  
    **Answer**: O(n)

37. **Question**: In a hash table with chaining, what is the average time complexity for search with n elements and m buckets?  
    **Solution**:  
    Average chain length = n/m. Search: O(n/m). If m ≈ n, O(1).  
    **Answer**: O(1) (assuming m ≈ n)

38. **Question**: In Python, what is the output of: `from collections import Counter; c = Counter([1, 2, 2, 3]); print(c[2])`?  
    **Solution**:  
    `Counter` counts occurrences. `c[2]` = 2 (two `2`s).  
    **Answer**: 2

39. **Question**: What is the time complexity to check if a binary tree is balanced?  
    **Solution**:  
    Compute height of each subtree, check difference: O(n).  
    **Answer**: O(n)

40. **Question**: In a stack, after push(1, 2, 3), pop(), push(4), pop(), what is the top element?  
    **Solution**:  
    Stack: Push `1, 2, 3`. Pop removes `3`. Push `4`. Pop removes `4`. Top: `2`.  
    **Answer**: 2

## Algorithms (41–60)

41. **Question**: What is the time complexity of merge sort for n elements?  
    **Solution**:  
    Divide and merge: O(n log n).  
    **Answer**: O(n log n)

42. **Question**: In Python, what is the output of this binary search: `def bs(arr, t): l, r = 0, len(arr)-1; while l <= r: m = (l+r)//2; if arr[m] == t: return m; elif arr[m] < t: l = m+1; else: r = m-1; return -1; print(bs([1, 2, 3, 4], 3))`?  
    **Solution**:  
    Binary search finds `3` at index `2`.  
    **Answer**: 2

43. **Question**: What is the space complexity of quicksort?  
    **Solution**:  
    Recursion stack: O(log n) average, O(n) worst case.  
    **Answer**: O(log n) (average)

44. **Question**: In C, what is the output of this GCD code: `int gcd(int a, int b) { if(b == 0) return a; return gcd(b, a % b); } printf("%d", gcd(48, 18));`?  
    **Solution**:  
    Euclidean algorithm: `gcd(48, 18) = gcd(18, 12) = gcd(12, 6) = gcd(6, 0) = 6`.  
    **Answer**: 6

45. **Question**: What is the time complexity of finding all pairs in an array of n elements that sum to a given value?  
    **Solution**:  
    Using a hash set: O(n). Without hash set: O(n²).  
    **Answer**: O(n) (with hash set)

46. **Question**: In Python, what is the output of: `x = [4, 2, 5, 1]; x.sort(); print(x)`?  
    **Solution**:  
    `sort()` sorts in-place: `[1, 2, 4, 5]`.  
    **Answer**: [1, 2, 4, 5]

47. **Question**: What is the time complexity of Dijkstra’s algorithm using a priority queue for a graph with V vertices and E edges?  
    **Solution**:  
    Priority queue operations: O((V + E) log V).  
    **Answer**: O((V + E) log V)

48. **Question**: In C++, what is the output of: `vector<int> v = {1, 2, 3}; rotate(v.begin(), v.begin()+1, v.end()); cout << v[0];`?  
    **Solution**:  
    `rotate` shifts left by 1: `[2, 3, 1]`. First element: `2`.  
    **Answer**: 2

49. **Question**: What is the time complexity of insertion sort for n elements?  
    **Solution**:  
    Compare and shift: O(n²).  
    **Answer**: O(n²)

50. **Question**: In Python, what is the output of: `x = [1, 2, 3, 4]; print([i for i in x if i % 2 == 0])`?  
    **Solution**:  
    List comprehension filters even numbers: `[2, 4]`.  
    **Answer**: [2, 4]

51. **Question**: What is the time complexity of checking if a string is a palindrome?  
    **Solution**:  
    Compare characters from both ends: O(n).  
    **Answer**: O(n)

52. **Question**: In C, what is the output of this Fibonacci code: `int fib(int n) { if(n <= 1) return n; return fib(n-1) + fib(n-2); } printf("%d", fib(5));`?  
    **Solution**:  
    `fib(5) = fib(4) + fib(3) = (fib(3) + fib(2)) + (fib(2) + fib(1)) = (2 + 1) + (1 + 1) = 5`.  
    **Answer**: 5

53. **Question**: What is the space complexity of merge sort?  
    **Solution**:  
    Extra array for merging: O(n).  
    **Answer**: O(n)

54. **Question**: In Python, what is the output of: `x = "hello"; print(''.join(reversed(x)))`?  
    **Solution**:  
    `reversed` reverses string: `"olleh"`.  
    **Answer**: olleh

55. **Question**: What is the time complexity of finding the longest common prefix of n strings of length m?  
    **Solution**:  
    Compare characters across strings: O(n * m).  
    **Answer**: O(n * m)

56. **Question**: In C++, what is the output of: `int arr[] = {1, 2, 3}; int *p = arr; cout << *(p + 2);`?  
    **Solution**:  
    `*(p + 2)` accesses `arr[2] = 3`.  
    **Answer**: 3

57. **Question**: What is the time complexity of counting sort for n elements with range k?  
    **Solution**:  
    Create count array and output: O(n + k).  
    **Answer**: O(n + k)

58. **Question**: In Python, what is the output of: `x = [1, 2, 2, 3]; print(list(set(x)))`?  
    **Solution**:  
    `set(x)` removes duplicates, `list` converts back: `[1, 2, 3]`.  
    **Answer**: [1, 2, 3]

59. **Question**: What is the time complexity of detecting a cycle in a linked list?  
    **Solution**:  
    Floyd’s cycle-finding algorithm (two pointers): O(n).  
    **Answer**: O(n)

60. **Question**: In C, what is the output of: `int arr[] = {3, 1, 4}; qsort(arr, 3, sizeof(int), [](const void* a, const void* b){return *(int*)a - *(int*)b;}); printf("%d", arr[0]);`?  
    **Solution**:  
    `qsort` sorts array: `[1, 3, 4]`. First element: `1`.  
    **Answer**: 1

## Database Basics (61–70)

61. **Question**: What is the result of this SQL query: `SELECT name, salary FROM employees WHERE department = 'IT' ORDER BY salary DESC;`?  
    **Solution**:  
    Retrieves `name` and `salary` for `department = 'IT'`, sorted by `salary` in descending order.  
    **Answer**: IT employees sorted by salary (highest first)

62. **Question**: What does `SELECT * FROM orders INNER JOIN customers ON orders.customer_id = customers.id;` do?  
    **Solution**:  
    Combines rows from `orders` and `customers` where `customer_id` matches `id`.  
    **Answer**: Joins orders with customer details

63. **Question**: What is the output of: `SELECT department, COUNT(*) FROM employees GROUP BY department;`?  
    **Solution**:  
    Counts employees per `department`.  
    **Answer**: Department-wise employee counts

64. **Question**: What does `FOREIGN KEY` constraint ensure in SQL?  
    **Solution**:  
    Ensures values in a column match values in another table’s primary key.  
    **Answer**: Referential integrity

65. **Question**: What is the result of: `SELECT product_name FROM products WHERE price BETWEEN 50 AND 100;`?  
    **Solution**:  
    Retrieves `product_name` where `price` is 50 to 100 (inclusive).  
    **Answer**: Products priced 50–100

66. **Question**: What does `SELECT DISTINCT city FROM customers;` do?  
    **Solution**:  
    Returns unique `city` values from `customers`.  
    **Answer**: Unique cities

67. **Question**: What is the output of: `SELECT name FROM students WHERE marks > (SELECT AVG(marks) FROM students);`?  
    **Solution**:  
    Retrieves `name` of students with `marks` above the average.  
    **Answer**: Students with above-average marks

68. **Question**: What does `ALTER TABLE employees ADD COLUMN email VARCHAR(100);` do?  
    **Solution**:  
    Adds an `email` column to `employees` table.  
    **Answer**: Adds email column

69. **Question**: What is the result of: `SELECT order_id, customer_name FROM orders LEFT JOIN customers ON orders.customer_id = customers.id;`?  
    **Solution**:  
    Includes all `orders`, with matching `customer_name` or NULL if no match.  
    **Answer**: All orders with customer names (or NULL)

70. **Question**: What does `CREATE INDEX idx_name ON employees(name);` do?  
    **Solution**:  
    Creates an index on `name` column to speed up queries.  
    **Answer**: Improves query performance

## Computer Networks (71–80)

71. **Question**: What is the purpose of the OSI model?  
    **Solution**:  
    Provides a framework for network communication with seven layers.  
    **Answer**: Standardizes network communication

72. **Question**: Which layer of the OSI model handles routing of packets?  
    **Solution**:  
    Network layer (Layer 3) manages routing.  
    **Answer**: Network layer

73. **Question**: What is the port number used by HTTPS?  
    **Solution**:  
    HTTPS uses port 443 for secure communication.  
    **Answer**: 443

74. **Question**: What is the purpose of NAT (Network Address Translation)?  
    **Solution**:  
    Maps private IP addresses to a public IP for internet access.  
    **Answer**: IP address mapping

75. **Question**: What is the difference between a hub and a switch?  
    **Solution**:  
    Hub broadcasts data to all ports; switch forwards data to specific devices.  
    **Answer**: Hub: broadcasts, Switch: targeted

76. **Question**: What is the role of the MAC address?  
    **Solution**:  
    Uniquely identifies a device at the data link layer.  
    **Answer**: Device identification

77. **Question**: What does the TCP three-way handshake involve?  
    **Solution**:  
    SYN, SYN-ACK, ACK to establish a connection.  
    **Answer**: Connection establishment

78. **Question**: What is the purpose of ICMP?  
    **Solution**:  
    Handles error messages and diagnostics (e.g., ping).  
    **Answer**: Error reporting

79. **Question**: What is the maximum number of hosts in a subnet with mask 255.255.255.240?  
    **Solution**:  
    `/28` (240 = 11110000) has 2⁴ = 16 addresses (14 hosts, 1 network, 1 broadcast).  
    **Answer**: 14

80. **Question**: What is the role of BGP in networking?  
    **Solution**:  
    Border Gateway Protocol routes data between autonomous systems.  
    **Answer**: Inter-domain routing

## Operating Systems (81–90)

81. **Question**: What is the difference between preemptive and non-preemptive scheduling?  
    **Solution**:  
    Preemptive: CPU can interrupt a process; Non-preemptive: process runs to completion.  
    **Answer**: Preemptive: interruptible, Non-preemptive: uninterruptible

82. **Question**: What is a semaphore in an operating system?  
    **Solution**:  
    Synchronization tool to control access to shared resources.  
    **Answer**: Synchronization mechanism

83. **Question**: What is the purpose of paging in memory management?  
    **Solution**:  
    Divides memory into fixed-size pages to simplify allocation.  
    **Answer**: Memory allocation

84. **Question**: What is the difference between a process and a thread?  
    **Solution**:  
    Process: independent program with own memory; Thread: lightweight, shares process memory.  
    **Answer**: Process: isolated, Thread: shared memory

85. **Question**: What is the role of the swap space in an OS?  
    **Solution**:  
    Disk space used to store inactive pages when RAM is full.  
    **Answer**: Extends virtual memory

86. **Question**: What is a context switch in an operating system?  
    **Solution**:  
    Saves current process state and loads another to switch execution.  
    **Answer**: Process switching

87. **Question**: What is the purpose of the LRU page replacement algorithm?  
    **Solution**:  
    Replaces the least recently used page to minimize page faults.  
    **Answer**: Optimizes page replacement

88. **Question**: What is a race condition in an OS?  
    **Solution**:  
    Occurs when multiple processes access shared data concurrently, leading to unpredictable results.  
    **Answer**: Concurrent access issue

89. **Question**: What is the role of the file allocation table (FAT) in a file system?  
    **Solution**:  
    Tracks file locations on disk.  
    **Answer**: File location tracking

90. **Question**: What is the purpose of a mutex in an OS?  
    **Solution**:  
    Ensures mutual exclusion to prevent concurrent access to critical sections.  
    **Answer**: Mutual exclusion

## AI/ML Foundations (91–100)

91. **Question**: What is the difference between classification and regression in ML?  
    **Solution**:  
    Classification predicts discrete labels; regression predicts continuous values.  
    **Answer**: Classification: labels, Regression: values

92. **Question**: What is the purpose of cross-validation in ML?  
    **Solution**:  
    Splits data into multiple folds to evaluate model performance robustly.  
    **Answer**: Robust model evaluation

93. **Question**: What is the bias-variance tradeoff in ML?  
    **Solution**:  
    High bias: underfitting; high variance: overfitting. Balance minimizes error.  
    **Answer**: Balances underfitting and overfitting

94. **Question**: What is the role of the learning rate in gradient descent?  
    **Solution**:  
    Controls step size for parameter updates during optimization.  
    **Answer**: Step size control

95. **Question**: What is the purpose of regularization in ML?  
    **Solution**:  
    Adds penalty to model complexity to prevent overfitting.  
    **Answer**: Prevents overfitting

96. **Question**: What is the difference between a perceptron and a multi-layer perceptron (MLP)?  
    **Solution**:  
    Perceptron: single-layer; MLP: multiple layers for non-linear problems.  
    **Answer**: Perceptron: single, MLP: multiple layers

97. **Question**: What is the purpose of the softmax function in neural networks?  
    **Solution**:  
    Converts logits to probabilities for multi-class classification.  
    **Answer**: Probability conversion

98. **Question**: What is the role of k in k-nearest neighbors (k-NN)?  
    **Solution**:  
    Number of neighbors considered for prediction.  
    **Answer**: Neighbor count

99. **Question**: What is the difference between bagging and boosting in ML?  
    **Solution**:  
    Bagging: parallel ensembles (e.g., Random Forest); Boosting: sequential, corrects errors (e.g., AdaBoost).  
    **Answer**: Bagging: parallel, Boosting: sequential

100. **Question**: What is the purpose of principal component analysis (PCA) in ML?  
     **Solution**:  
     Reduces dimensionality by projecting data onto principal components.  
     **Answer**: Dimensionality reduction