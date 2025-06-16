# 100 Technical Aptitude Practice Questions (Advanced Level) with Solutions

This file contains **100 advanced-level practice questions** for Technical Aptitude, designed to rigorously test and enhance technical knowledge and problem-solving skills for fresher job aptitude tests, especially for AI/ML roles. Each question includes a detailed description of the problem (e.g., complex programming, advanced data structures, algorithms, databases, networks, operating systems, AI/ML) and a comprehensive solution explaining the reasoning process. Topics cover dynamic programming, graph algorithms, advanced SQL, network security, concurrency, and AI/ML model optimization.

## Programming Fundamentals (1–20)

1. **Question**: What is the output of this C code: `int x = 5; int *p = &x; *p += 2; printf("%d %d", x, *p);`?  
   **Solution**:  
   `p` points to `x`. `*p += 2` modifies `x` to `5 + 2 = 7`. Both `x` and `*p` access the same memory. Output: `7 7`.  
   **Answer**: 7 7

2. **Question**: In Python, what is the output of: `x = [[0]*2]*3; x[0][0] = 1; print(x)`?  
   **Solution**:  
   `[[0]*2]*3` creates three references to the same inner list. Modifying `x[0][0]` affects all rows. Output: `[[1, 0], [1, 0], [1, 0]]`.  
   **Answer**: [[1, 0], [1, 0], [1, 0]]

3. **Question**: In Java, what is the output of: `String s1 = new String("test"); String s2 = new String("test"); System.out.println(s1 == s2);`?  
   **Solution**:  
   `==` checks reference equality. `new String` creates distinct objects. Output: `false`.  
   **Answer**: false

4. **Question**: In C++, what is the output of: `int x = 10; auto f = [&x]() { x += 5; return x; }; cout << f() << " " << x;`?  
   **Solution**:  
   Lambda captures `x` by reference. `f()` increments `x` to `15`, returns `15`. `x` is also `15`. Output: `15 15`.  
   **Answer**: 15 15

5. **Question**: In Python, what is the output of: `def f(x=[]): x.append(1); return x; print(f(), f())`?  
   **Solution**:  
   Default list `x` is shared across calls. First `f()`: `x = [1]`. Second `f()`: `x = [1, 1]`. Output: `[1] [1, 1]`.  
   **Answer**: [1] [1, 1]

6. **Question**: In C, what is the output of: `int x = 5; void *p = &x; printf("%d", *(int*)p);`?  
   **Solution**:  
   `p` is a void pointer to `x`. Cast to `int*` and dereference gives `5`. Output: `5`.  
   **Answer**: 5

7. **Question**: In Java, what is the output of: `Integer a = 127; Integer b = 127; System.out.println(a == b);`?  
   **Solution**:  
   Integer caching for `-128` to `127` reuses objects. `a` and `b` reference the same object. Output: `true`.  
   **Answer**: true

8. **Question**: In Python, what is the output of: `x = {1: [1], 2: [2]}; y = x.copy(); y[1].append(3); print(x[1])`?  
   **Solution**:  
   `copy()` creates a shallow copy. `y[1]` references the same list as `x[1]`. Appending `3` modifies `x[1]`. Output: `[1, 3]`.  
   **Answer**: [1, 3]

9. **Question**: In C++, what is the output of: `int arr[] = {1, 2, 3}; int *p = arr; cout << *(p + 1) * *(p + 2);`?  
   **Solution**:  
   `*(p + 1) = arr[1] = 2`, `*(p + 2) = arr[2] = 3`. `2 * 3 = 6`. Output: `6`.  
   **Answer**: 6

10. **Question**: In C, what is the output of: `union U { int x; char c; } u; u.x = 258; printf("%d", u.c);`?  
    **Solution**:  
    Union shares memory. `x = 258` (binary `00000001 00000010`). `c` reads first byte (`00000010` = 2). Output: `2`.  
    **Answer**: 2

11. **Question**: In Python, what is the output of: `from functools import reduce; print(reduce(lambda x, y: x + y, [1, 2, 3], 0))`?  
    **Solution**:  
    `reduce` applies `+` with initial value `0`: `((0 + 1) + 2) + 3 = 6`. Output: `6`.  
    **Answer**: 6

12. **Question**: In Java, what is the output of: `try { throw new Exception("Error"); } catch (Exception e) { System.out.println("Caught"); } finally { System.out.println("Finally"); }`?  
    **Solution**:  
    Exception is caught, prints `Caught`. `finally` always executes. Output: `Caught Finally`.  
    **Answer**: Caught Finally

13. **Question**: In C++, what is the output of: `vector<int> v = {1, 2, 3}; transform(v.begin(), v.end(), v.begin(), [](int x) { return x * x; }); cout << v[1];`?  
    **Solution**:  
    `transform` squares each element. `v = [1, 4, 9]`. `v[1] = 4`. Output: `4`.  
    **Answer**: 4

14. **Question**: In Python, what is the output of: `x = [1, 2, 3]; y = iter(x); next(y); print(next(y))`?  
    **Solution**:  
    `iter(x)` creates an iterator. First `next(y)` returns `1`. Second `next(y)` returns `2`. Output: `2`.  
    **Answer**: 2

15. **Question**: In C, what is the output of: `int x = 5; int y = x++ + ++x; printf("%d %d", x, y);`?  
    **Solution**:  
    Undefined behavior due to multiple modifications of `x` without sequence point. Possible: `x = 7`, `y = 12` (5 + 7). Output varies, assume common compiler: `7 12`.  
    **Answer**: 7 12 (compiler-dependent)

16. **Question**: In Java, what is the output of: `List<Integer> list = Arrays.asList(1, 2, 3); list.replaceAll(x -> x + 1); System.out.println(list);`?  
    **Solution**:  
    `replaceAll` increments each element. `list = [2, 3, 4]`. Output: `[2, 3, 4]`.  
    **Answer**: [2, 3, 4]

17. **Question**: In Python, what is the output of: `import copy; x = [[1], [2]]; y = copy.deepcopy(x); y[0].append(3); print(x)`?  
    **Solution**:  
    `deepcopy` creates independent copies. Modifying `y` doesn’t affect `x`. Output: `[[1], [2]]`.  
    **Answer**: [[1], [2]]

18. **Question**: In C++, what is the output of: `int x = 5; function<int(int)> f = [&](int a) { x += a; return x; }; cout << f(3);`?  
    **Solution**:  
    Lambda captures `x` by reference. `f(3)` adds `3` to `x = 5`, returns `x = 8`. Output: `8`.  
    **Answer**: 8

19. **Question**: In C, what is the output of: `struct S { int x; char c; } s = {10, 'A'}; printf("%d %c", s.x, s.c);`?  
    **Solution**:  
    `s.x = 10`, `s.c = 'A'`. Output: `10 A`.  
    **Answer**: 10 A

20. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(list(filter(lambda x: x % 2 == 1, x)))`?  
    **Solution**:  
    `filter` selects odd numbers: `[1, 3]`. Output: `[1, 3]`.  
    **Answer**: [1, 3]

## Data Structures (21–40)

21. **Question**: What is the time complexity of finding the lowest common ancestor (LCA) in a binary search tree with n nodes?  
    **Solution**:  
    Traverse from root to nodes, comparing values: O(h), where h is height (O(log n) if balanced).  
    **Answer**: O(log n) (balanced)

22. **Question**: In Python, what is the output of this AVL tree insertion (simplified): `class Node: def __init__(self, val): self.val = val; self.left = self.right = None; root = Node(10); root.left = Node(5); root.right = Node(15); root.right.right = Node(20); print(root.right.right.val)`?  
    **Solution**:  
    Tree structure: `10 -> 15 -> 20`. `root.right.right.val = 20`. Output: `20`.  
    **Answer**: 20

23. **Question**: What is the time complexity of building a binary heap from an array of n elements?  
    **Solution**:  
    Heapify from bottom-up: O(n).  
    **Answer**: O(n)

24. **Question**: In a graph with V vertices and E edges, what is the time complexity of detecting a cycle using DFS?  
    **Solution**:  
    DFS visits all vertices and edges: O(V + E).  
    **Answer**: O(V + E)

25. **Question**: In Python, what is the output of: `from collections import defaultdict; d = defaultdict(list); d[1].append(2); d[1].append(3); print(d)`?  
    **Solution**:  
    `defaultdict` creates empty list for new keys. `d[1] = [2, 3]`. Output: `defaultdict(<class 'list'>, {1: [2, 3]})`.  
    **Answer**: defaultdict(<class 'list'>, {1: [2, 3]})

26. **Question**: What is the time complexity of finding the shortest path in an unweighted graph using BFS?  
    **Solution**:  
    BFS explores all vertices and edges: O(V + E).  
    **Answer**: O(V + E)

27. **Question**: In a trie with n words of average length k, what is the time complexity to search for a word?  
    **Solution**:  
    Traverse characters: O(k).  
    **Answer**: O(k)

28. **Question**: In Python, what is the output of: `class Node: def __init__(self, val): self.val = val; self.next = None; head = Node(1); head.next = Node(2); head.next.next = Node(3); print(head.next.next.val)`?  
    **Solution**:  
    Linked list: `1 -> 2 -> 3`. `head.next.next.val = 3`. Output: `3`.  
    **Answer**: 3

29. **Question**: What is the time complexity of Kruskal’s algorithm for minimum spanning tree with V vertices and E edges?  
    **Solution**:  
    Sort edges O(E log E), union-find O(E α(V)) ≈ O(E log V). Total: O(E log V).  
    **Answer**: O(E log V)

30. **Question**: In a segment tree for range sum queries with n elements, what is the time complexity of a query?  
    **Solution**:  
    Traverse height of tree: O(log n).  
    **Answer**: O(log n)

31. **Question**: In Python, what is the output of: `from heapq import heappush, heappop; h = []; heappush(h, 3); heappush(h, 1); heappush(h, 2); print(heappop(h))`?  
    **Solution**:  
    Min-heap: `[1, 2, 3]`. `heappop` removes smallest: `1`. Output: `1`.  
    **Answer**: 1

32. **Question**: What is the time complexity of deleting a node from a red-black tree with n nodes?  
    **Solution**:  
    Rebalance after deletion: O(log n).  
    **Answer**: O(log n)

33. **Question**: In a weighted graph, what is the time complexity of Bellman-Ford algorithm for single-source shortest paths?  
    **Solution**:  
    Relax edges V-1 times: O(V * E).  
    **Answer**: O(V * E)

34. **Question**: In Python, what is the output of: `from collections import deque; g = {1: [2, 3], 2: [4], 3: [4], 4: []}; q = deque([1]); visited = {1}; while q: n = q.popleft(); for nei in g[n]: if nei not in visited: visited.add(nei); q.append(nei); print(len(visited))`?  
    **Solution**:  
    BFS visits all nodes in graph: `1, 2, 3, 4`. `len(visited) = 4`. Output: `4`.  
    **Answer**: 4

35. **Question**: What is the space complexity of storing a sparse graph with V vertices and E edges?  
    **Solution**:  
    Adjacency list: O(V + E).  
    **Answer**: O(V + E)

36. **Question**: In a B-tree of order m with n keys, what is the time complexity of searching a key?  
    **Solution**:  
    Traverse height: O(log_m n).  
    **Answer**: O(log n)

37. **Question**: In Python, what is the output of: `x = [(1, 'a'), (2, 'b'), (1, 'c')]; x.sort(); print(x)`?  
    **Solution**:  
    Sort by first element, then second: `[(1, 'a'), (1, 'c'), (2, 'b')]`. Output: `[(1, 'a'), (1, 'c'), (2, 'b')]`.  
    **Answer**: [(1, 'a'), (1, 'c'), (2, 'b')]

38. **Question**: What is the time complexity of finding strongly connected components using Kosaraju’s algorithm?  
    **Solution**:  
    Two DFS passes and transpose: O(V + E).  
    **Answer**: O(V + E)

39. **Question**: In a suffix tree for a string of length n, what is the time complexity to check if a substring exists?  
    **Solution**:  
    Traverse path matching substring: O(m), where m is substring length.  
    **Answer**: O(m)

40. **Question**: In Python, what is the output of: `from collections import OrderedDict; d = OrderedDict([(1, 'a'), (2, 'b')]); d.move_to_end(1); print(list(d.keys()))`?  
    **Solution**:  
    `move_to_end(1)` moves key `1` to end. Keys: `[2, 1]`. Output: `[2, 1]`.  
    **Answer**: [2, 1]

## Algorithms (41–60)

41. **Question**: What is the time complexity of the knapsack problem (0/1) using dynamic programming for n items and capacity W?  
    **Solution**:  
    DP table of size n × W: O(n * W).  
    **Answer**: O(n * W)

42. **Question**: In Python, what is the output of this longest common subsequence: `def lcs(s1, s2): m, n = len(s1), len(s2); dp = [[0]*(n+1) for _ in range(m+1)]; for i in range(1, m+1): for j in range(1, n+1): if s1[i-1] == s2[j-1]: dp[i][j] = dp[i-1][j-1] + 1; else: dp[i][j] = max(dp[i-1][j], dp[i][j-1]); return dp[m][n]; print(lcs("ABC", "AC"))`?  
    **Solution**:  
    LCS of `"ABC"` and `"AC"` is `"AC"`. Length: `2`. Output: `2`.  
    **Answer**: 2

43. **Question**: What is the time complexity of matrix chain multiplication for n matrices using dynamic programming?  
    **Solution**:  
    DP table for all possible splits: O(n³).  
    **Answer**: O(n³)

44. **Question**: In C++, what is the output of: `vector<int> v = {3, 1, 4, 1, 5}; int k = 2; multiset<int> s(v.begin(), v.begin()+k); int ans = *s.rbegin(); for(int i = k; i < v.size(); i++) { s.erase(s.find(v[i-k])); s.insert(v[i]); ans = max(ans, *s.rbegin()); } cout << ans;`?  
    **Solution**:  
    Sliding window maximum using multiset. Max of `[3,1], [1,4], [4,1], [1,5]` is `4`. Output: `4`.  
    **Answer**: 4

45. **Question**: What is the time complexity of Floyd-Warshall algorithm for all-pairs shortest paths in a graph with V vertices?  
    **Solution**:  
    Three nested loops: O(V³).  
    **Answer**: O(V³)

46. **Question**: In Python, what is the output of: `def kadane(arr): max_so_far = max_ending_here = arr[0]; for x in arr[1:]: max_ending_here = max(x, max_ending_here + x); max_so_far = max(max_so_far, max_ending_here); return max_so_far; print(kadane([-2, 1, -3, 4, -1, 2, 1]))`?  
    **Solution**:  
    Kadane’s algorithm finds max subarray sum: `[4, -1, 2, 1] = 6`. Output: `6`.  
    **Answer**: 6

47. **Question**: What is the time complexity of finding the median of two sorted arrays of size n each?  
    **Solution**:  
    Binary search to partition arrays: O(log n).  
    **Answer**: O(log n)

48. **Question**: In C, what is the output of this KMP preprocessing: `void computeLPS(char *pat, int m, int *lps) { int len = 0, i = 1; lps[0] = 0; while(i < m) { if(pat[i] == pat[len]) { len++; lps[i++] = len; } else if(len > 0) len = lps[len-1]; else lps[i++] = 0; } } int lps[6]; computeLPS("AABAAC", 6, lps); printf("%d", lps[5]);`?  
    **Solution**:  
    LPS for `"AABAAC"`: `[0, 1, 0, 1, 2, 0]`. `lps[5] = 0`. Output: `0`.  
    **Answer**: 0

49. **Question**: What is the time complexity of the A* search algorithm in a graph?  
    **Solution**:  
    Depends on heuristic, typically O(b^d) where b is branching factor, d is depth.  
    **Answer**: O(b^d)

50. **Question**: In Python, what is the output of: `def edit_distance(s1, s2): m, n = len(s1), len(s2); dp = [[0]*(n+1) for _ in range(m+1)]; for i in range(m+1): dp[i][0] = i; for j in range(n+1): dp[0][j] = j; for i in range(1, m+1): for j in range(1, n+1): if s1[i-1] == s2[j-1]: dp[i][j] = dp[i-1][j-1]; else: dp[i][j] = min(dp[i-1][j], dp[i][j-1], dp[i-1][j-1]) + 1; return dp[m][n]; print(edit_distance("cat", "cut"))`?  
    **Solution**:  
    Edit distance from `"cat"` to `"cut"` is 1 (replace `a` with `u`). Output: `1`.  
    **Answer**: 1

51. **Question**: What is the time complexity of finding the longest palindromic substring using dynamic programming?  
    **Solution**:  
    DP table for all substrings: O(n²).  
    **Answer**: O(n²)

52. **Question**: In C++, what is the output of: `int n = 5; vector<vector<int>> dp(n+1, vector<int>(n+1)); for(int i = 0; i <= n; i++) dp[i][0] = dp[0][i] = 1; for(int i = 1; i <= n; i++) for(int j = 1; j <= n; j++) dp[i][j] = dp[i-1][j] + dp[i][j-1]; cout << dp[n][n];`?  
    **Solution**:  
    DP computes number of paths in n×n grid: `dp[5][5] = 252` (binomial coefficient). Output: `252`.  
    **Answer**: 252

53. **Question**: What is the space complexity of the Rabin-Karp string matching algorithm?  
    **Solution**:  
    Rolling hash and pattern storage: O(1) extra space.  
    **Answer**: O(1)

54. **Question**: In Python, what is the output of: `def max_profit(prices): n = len(prices); if n < 2: return 0; dp = [0]*n; min_price = prices[0]; for i in range(1, n): min_price = min(min_price, prices[i]); dp[i] = max(dp[i-1], prices[i] - min_price); return dp[n-1]; print(max_profit([7, 1, 5, 3, 6, 4]))`?  
    **Solution**:  
    Max profit by buying at `1`, selling at `6`: `6 - 1 = 5`. Output: `5`.  
    **Answer**: 5

55. **Question**: What is the time complexity of computing the convex hull of n points using Graham’s scan?  
    **Solution**:  
    Sort points O(n log n), scan O(n). Total: O(n log n).  
    **Answer**: O(n log n)

56. **Question**: In C, what is the output of: `int n = 4; int dp[5]; dp[0] = 1; for(int i = 1; i <= n; i++) { dp[i] = 0; for(int j = 0; j < i; j++) dp[i] += dp[j] * dp[i-j-1]; } printf("%d", dp[n]);`?  
    **Solution**:  
    Catalan number for `n = 4`: `dp[4] = 14` (number of BSTs). Output: `14`.  
    **Answer**: 14

57. **Question**: What is the time complexity of the Hungarian algorithm for bipartite matching with n vertices?  
    **Solution**:  
    Maximum flow approach: O(n³).  
    **Answer**: O(n³)

58. **Question**: In Python, what is the output of: `def count_inversions(arr): def merge_and_count(l, r): inv = 0; res = []; i = j = 0; while i < len(l) and j < len(r): if l[i] <= r[j]: res.append(l[i]); i += 1; else: res.append(r[j]); inv += len(l)-i; j += 1; res.extend(l[i:]); res.extend(r[j:]); return res, inv; def sort_and_count(arr): if len(arr) <= 1: return arr, 0; mid = len(arr)//2; l, inv_l = sort_and_count(arr[:mid]); r, inv_r = sort_and_count(arr[mid:]); merged, inv_m = merge_and_count(l, r); return merged, inv_l + inv_r + inv_m; _, inv = sort_and_count([3, 1, 2]); print(inv)`?  
    **Solution**:  
    Inversions in `[3, 1, 2]`: `(3, 1), (3, 2)`. Count: `2`. Output: `2`.  
    **Answer**: 2

59. **Question**: What is the time complexity of finding the k-th smallest element in two sorted arrays of sizes m and n?  
    **Solution**:  
    Binary search on partitions: O(log(min(m, n))).  
    **Answer**: O(log(min(m, n)))

60. **Question**: In C++, what is the output of: `int n = 3; vector<int> dp(n+1); dp[0] = 1; for(int i = 1; i <= n; i++) for(int j = 1; j <= i; j++) dp[i] += dp[i-j]; cout << dp[n];`?  
    **Solution**:  
    Number of ways to sum to `n` with positive integers: `dp[3] = 4` (1+1+1, 1+2, 2+1, 3). Output: `4`.  
    **Answer**: 4

## Database Basics (61–70)

61. **Question**: What is the result of this SQL query: `SELECT d.department_name, AVG(e.salary) FROM employees e JOIN departments d ON e.department_id = d.id GROUP BY d.department_name HAVING COUNT(e.id) > 5 ORDER BY AVG(e.salary) DESC;`?  
    **Solution**:  
    Joins `employees` and `departments`, groups by `department_name`, computes average `salary`, filters departments with >5 employees, sorts by average salary descending.  
    **Answer**: Department names and average salaries for departments with >5 employees, sorted high to low

62. **Question**: What does `SELECT c.customer_name, COUNT(o.order_id) FROM customers c LEFT JOIN orders o ON c.id = o.customer_id GROUP BY c.customer_name;` do?  
    **Solution**:  
    Counts orders per customer, including customers with zero orders.  
    **Answer**: Customer names and their order counts

63. **Question**: What is the output of: `SELECT product_name, price FROM products WHERE price > (SELECT AVG(price) FROM products WHERE category = products.category);`?  
    **Solution**:  
    Retrieves `product_name` and `price` for products priced above their category’s average.  
    **Answer**: Products above category average price

64. **Question**: What does `CREATE TRIGGER update_stock AFTER INSERT ON orders FOR EACH ROW UPDATE products SET stock = stock - NEW.quantity WHERE id = NEW.product_id;` do?  
    **Solution**:  
    Automatically reduces `stock` in `products` by `quantity` after an order is inserted.  
    **Answer**: Updates product stock on order insertion

65. **Question**: What is the result of: `SELECT e1.name FROM employees e1 WHERE e1.salary > (SELECT AVG(e2.salary) FROM employees e2 WHERE e2.manager_id = e1.id);`?  
    **Solution**:  
    Retrieves names of employees with salaries above the average salary of their direct reports.  
    **Answer**: Employees earning above their team’s average

66. **Question**: What does `EXPLAIN SELECT * FROM orders WHERE customer_id = 100;` do?  
    **Solution**:  
    Provides query execution plan, showing how the database processes the query.  
    **Answer**: Shows query plan

67. **Question**: What is the output of: `SELECT category, MAX(price) FROM products GROUP BY category UNION SELECT 'Total', MAX(price) FROM products;`?  
    **Solution**:  
    Lists maximum `price` per `category`, plus overall maximum `price` labeled as `'Total'`.  
    **Answer**: Category max prices and overall max price

68. **Question**: What does `ALTER TABLE employees ADD CONSTRAINT unique_email UNIQUE (email);` do?  
    **Solution**:  
    Adds a unique constraint to `email` column, preventing duplicate emails.  
    **Answer**: Enforces unique emails

69. **Question**: What is the result of: `SELECT name FROM students s WHERE EXISTS (SELECT 1 FROM courses c WHERE c.student_id = s.id AND c.grade = 'A');`?  
    **Solution**:  
    Retrieves `name` of students who have at least one course with grade `'A'`.  
    **Answer**: Students with A-grade courses

70. **Question**: What does `CREATE VIEW high_salary AS SELECT name, salary FROM employees WHERE salary > 100000;` do?  
    **Solution**:  
    Creates a virtual table showing `name` and `salary` for employees with `salary > 100000`.  
    **Answer**: Creates high-salary view

## Computer Networks (71–80)

71. **Question**: What is the purpose of the Transport layer in the OSI model?  
    **Solution**:  
    Provides reliable data transfer, flow control, and error correction.  
    **Answer**: Reliable data transfer

72. **Question**: What is the role of IPSec in network security?  
    **Solution**:  
    Provides encryption and authentication for IP packets.  
    **Answer**: Secures IP communication

73. **Question**: What is the difference between TCP and SCTP?  
    **Solution**:  
    TCP: single stream, reliable; SCTP: multi-stream, supports multi-homing.  
    **Answer**: TCP: single stream, SCTP: multi-stream

74. **Question**: What is the purpose of the DHCP protocol?  
    **Solution**:  
    Dynamically assigns IP addresses to devices on a network.  
    **Answer**: IP address assignment

75. **Question**: What is the role of the TTL field in an IP header?  
    **Solution**:  
    Limits packet lifetime to prevent infinite loops (decremented per hop).  
    **Answer**: Prevents routing loops

76. **Question**: What is the difference between stateful and stateless firewalls?  
    **Solution**:  
    Stateful: tracks connection states; Stateless: filters packets based on rules.  
    **Answer**: Stateful: connection-aware, Stateless: rule-based

77. **Question**: What is the purpose of the RST flag in TCP?  
    **Solution**:  
    Resets a connection due to errors or invalid segments.  
    **Answer**: Connection reset

78. **Question**: What is the role of SNMP in network management?  
    **Solution**:  
    Simple Network Management Protocol monitors and manages network devices.  
    **Answer**: Network monitoring

79. **Question**: What is the maximum throughput of a network with 100 Mbps bandwidth and 10 ms RTT, assuming TCP with window size 64 KB?  
    **Solution**:  
    Throughput = Window Size / RTT = (64 * 1024 * 8) / (10 / 1000) = 51.2 Mbps.  
    **Answer**: 51.2 Mbps

80. **Question**: What is the purpose of VLAN tagging in Ethernet networks?  
    **Solution**:  
    Adds identifiers to frames to separate traffic on virtual LANs.  
    **Answer**: Separates VLAN traffic

## Operating Systems (81–90)

81. **Question**: What is the difference between spinlock and semaphore in an OS?  
    **Solution**:  
    Spinlock: busy-waits in a loop; Semaphore: blocks threads, supports counting.  
    **Answer**: Spinlock: busy-wait, Semaphore: blocking

82. **Question**: What is the role of the TLB (Translation Lookaside Buffer) in virtual memory?  
    **Solution**:  
    Caches recent virtual-to-physical address translations to speed up access.  
    **Answer**: Speeds address translation

83. **Question**: What is the Banker’s algorithm used for in an OS?  
    **Solution**:  
    Prevents deadlock by ensuring safe resource allocation.  
    **Answer**: Deadlock avoidance

84. **Question**: What is the difference between user-level and kernel-level threads?  
    **Solution**:  
    User-level: managed by application, no kernel involvement; Kernel-level: OS-managed, supports parallelism.  
    **Answer**: User-level: app-managed, Kernel-level: OS-managed

85. **Question**: What is the purpose of copy-on-write in memory management?  
    **Solution**:  
    Delays copying shared memory pages until a write occurs, saving resources.  
    **Answer**: Optimizes memory usage

86. **Question**: What is the role of the inverted page table in an OS?  
    **Solution**:  
    Maps physical pages to virtual pages, reducing memory overhead.  
    **Answer**: Efficient page mapping

87. **Question**: What is the difference between hard and soft real-time systems?  
    **Solution**:  
    Hard: strict deadlines, failure is critical; Soft: deadlines important but not critical.  
    **Answer**: Hard: critical, Soft: non-critical

88. **Question**: What is the purpose of the monitor in process synchronization?  
    **Solution**:  
    Ensures mutual exclusion and provides condition variables for synchronization.  
    **Answer**: Synchronization construct

89. **Question**: What is the role of the I/O scheduler in an OS?  
    **Solution**:  
    Optimizes disk access by reordering I/O requests.  
    **Answer**: Optimizes disk I/O

90. **Question**: What is the difference between demand paging and prepaging?  
    **Solution**:  
    Demand paging: loads pages on demand; Prepaging: loads pages in advance to reduce faults.  
    **Answer**: Demand: on-demand, Prepaging: anticipatory

## AI/ML Foundations (91–100)

91. **Question**: What is the difference between L1 and L2 regularization in ML?  
    **Solution**:  
    L1: adds absolute weights (sparsity); L2: adds squared weights (smoothness).  
    **Answer**: L1: sparsity, L2: smoothness

92. **Question**: What is the purpose of early stopping in neural network training?  
    **Solution**:  
    Halts training when validation performance stops improving to prevent overfitting.  
    **Answer**: Prevents overfitting

93. **Question**: What is the role of batch normalization in deep learning?  
    **Solution**:  
    Normalizes layer inputs to stabilize and accelerate training.  
    **Answer**: Stabilizes training

94. **Question**: What is the difference between precision and recall in ML evaluation?  
    **Solution**:  
    Precision: TP/(TP+FP) (accuracy of positive predictions); Recall: TP/(TP+FN) (coverage of actual positives).  
    **Answer**: Precision: accuracy, Recall: coverage

95. **Question**: What is the purpose of dropout in neural networks?  
    **Solution**:  
    Randomly deactivates neurons during training to prevent overfitting.  
    **Answer**: Reduces overfitting

96. **Question**: What is the difference between CNN and RNN architectures?  
    **Solution**:  
    CNN: processes spatial data (e.g., images); RNN: processes sequential data (e.g., time series).  
    **Answer**: CNN: spatial, RNN: sequential

97. **Question**: What is the role of the attention mechanism in transformers?  
    **Solution**:  
    Weights input elements based on relevance, improving context understanding.  
    **Answer**: Focuses on relevant inputs

98. **Question**: What is the purpose of the F1 score in ML evaluation?  
    **Solution**:  
    Harmonic mean of precision and recall, balances both metrics.  
    **Answer**: Balances precision and recall

99. **Question**: What is the difference between generative and discriminative models in ML?  
    **Solution**:  
    Generative: models joint probability P(x,y); Discriminative: models conditional P(y|x).  
    **Answer**: Generative: joint, Discriminative: conditional

100. **Question**: What is the purpose of transfer learning in deep learning?  
     **Solution**:  
     Uses pre-trained models to improve performance on new tasks with less data.  
     **Answer**: Leverages pre-trained models