# 100 Data Interpretation Practice Questions (Advanced Level) with Solutions

This file contains **100 advanced-level practice questions** for Data Interpretation, designed to rigorously test your ability to analyze complex datasets for fresher job aptitude tests, especially for AI/ML roles. Each question includes a dataset (multiple tables, stacked bar graphs, combination charts, pie charts with secondary data, or caselets) and a detailed solution with step-by-step calculations. Topics cover compound growth rates, weighted averages, trend analysis, multi-dataset integration, percentages, ratios, and advanced comparisons.

## Multiple Table-Based Questions (1–20)

**Table 1: Annual Sales (in $1000) of Three Products Across Two Regions (2021–2023)**  
| Product | Region A (2021) | Region A (2022) | Region A (2023) | Region B (2021) | Region B (2022) | Region B (2023) |
|---------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| X       | 500             | 550             | 600             | 400             | 450             | 500             |
| Y       | 300             | 320             | 350             | 250             | 270             | 300             |
| Z       | 200             | 220             | 250             | 150             | 180             | 200             |

**Table 2: Unit Price ($ per unit) of Products (2021–2023)**  
| Product | 2021 | 2022 | 2023 |
|---------|------|------|------|
| X       | 10   | 12   | 15   |
| Y       | 8    | 9    | 10   |
| Z       | 5    | 6    | 7    |

1. **Question**: What is the total revenue from Product X in Region A in 2023?  
   **Solution**:  
   Sales = 600 ($1000) = 600,000. Units = 600,000 ÷ 15 = 40,000. Revenue = 40,000 × 15 = $600,000.  
   **Answer**: $600,000

2. **Question**: Which product had the highest revenue in Region B in 2022?  
   **Solution**:  
   X: 450,000 ÷ 12 = 37,500 units × 12 = $450,000.  
   Y: 270,000 ÷ 9 = 30,000 units × 9 = $270,000.  
   Z: 180,000 ÷ 6 = 30,000 units × 6 = $180,000.  
   Highest is X.  
   **Answer**: Product X

3. **Question**: What is the compound annual growth rate (CAGR) of Product Y’s sales in Region A from 2021 to 2023?  
   **Solution**:  
   Initial (2021) = 300 ($1000), Final (2023) = 350 ($1000).  
   CAGR = [(350 ÷ 300)^(1/2) - 1] × 100 ≈ [(1.1667)^0.5 - 1] × 100 ≈ 8.01%.  
   **Answer**: 8.01%

4. **Question**: What is the weighted average unit price of all products in 2022, weighted by units sold in Region A?  
   **Solution**:  
   Units X: 550,000 ÷ 12 ≈ 45,833. Y: 320,000 ÷ 9 ≈ 35,556. Z: 220,000 ÷ 6 ≈ 36,667.  
   Total units = 45,833 + 35,556 + 36,667 ≈ 118,056.  
   Weighted price = [(45,833 × 12) + (35,556 × 9) + (36,667 × 6)] ÷ 118,056 ≈ $9.26.  
   **Answer**: $9.26

5. **Question**: What is the total revenue across both regions for Product Z in 2021?  
   **Solution**:  
   A: 200,000 ÷ 5 = 40,000 units × 5 = $200,000.  
   B: 150,000 ÷ 5 = 30,000 units × 5 = $150,000.  
   Total = 200,000 + 150,000 = $350,000.  
   **Answer**: $350,000

6. **Question**: What is the percentage contribution of Product X to total revenue in Region B in 2023?  
   **Solution**:  
   X: 500,000 ÷ 15 ≈ 33,333 units × 15 = $500,000.  
   Y: 300,000 ÷ 10 = 30,000 units × 10 = $300,000.  
   Z: 200,000 ÷ 7 ≈ 28,571 units × 7 ≈ $200,000.  
   Total = 500,000 + 300,000 + 200,000 = $1,000,000.  
   % X = (500,000 ÷ 1,000,000) × 100 = 50%.  
   **Answer**: 50%

7. **Question**: What is the ratio of units sold of Product Y in Region A to Region B in 2022?  
   **Solution**:  
   A: 320,000 ÷ 9 ≈ 35,556 units. B: 270,000 ÷ 9 = 30,000 units.  
   Ratio = 35,556 : 30,000 ≈ 1.19 : 1 ≈ 119 : 100.  
   **Answer**: 119 : 100

8. **Question**: Which region showed the highest revenue growth for Product Z from 2021 to 2023?  
   **Solution**:  
   A: 2021: 200,000, 2023: 250,000. % Growth = (50 ÷ 200) × 100 = 25%.  
   B: 2021: 150,000, 2023: 200,000. % Growth = (50 ÷ 150) × 100 ≈ 33.33%.  
   B is higher.  
   **Answer**: Region B

9. **Question**: What is the total revenue of all products in Region A in 2022?  
   **Solution**:  
   X: 550,000. Y: 320,000. Z: 220,000. Total = 550,000 + 320,000 + 220,000 = $1,090,000.  
   **Answer**: $1,090,000

10. **Question**: What is the percentage increase in unit price of Product X from 2021 to 2023?  
    **Solution**:  
    Increase = 15 - 10 = 5. % Increase = (5 ÷ 10) × 100 = 50%.  
    **Answer**: 50%

**Table 3: Production Costs ($ per unit) and Units Produced (2021–2023)**  
| Product | Cost (2021) | Cost (2022) | Cost (2023) | Units (2021) | Units (2022) | Units (2023) |
|---------|-------------|-------------|-------------|--------------|--------------|--------------|
| P       | 4           | 5           | 6           | 20,000       | 22,000       | 25,000       |
| Q       | 6           | 7           | 8           | 15,000       | 18,000       | 20,000       |

11. **Question**: What is the total production cost of Product P in 2022?  
    **Solution**:  
    Cost = 22,000 × 5 = $110,000.  
    **Answer**: $110,000

12. **Question**: What is the percentage increase in production cost per unit for Product Q from 2021 to 2023?  
    **Solution**:  
    Increase = 8 - 6 = 2. % Increase = (2 ÷ 6) × 100 ≈ 33.33%.  
    **Answer**: 33.33%

13. **Question**: What is the total cost of producing both products in 2023?  
    **Solution**:  
    P: 25,000 × 6 = $150,000. Q: 20,000 × 8 = $160,000. Total = 150,000 + 160,000 = $310,000.  
    **Answer**: $310,000

14. **Question**: What is the CAGR of units produced for Product P from 2021 to 2023?  
    **Solution**:  
    Initial = 20,000, Final = 25,000. CAGR = [(25,000 ÷ 20,000)^(1/2) - 1] × 100 ≈ 11.80%.  
    **Answer**: 11.80%

15. **Question**: What is the ratio of total production costs of P to Q in 2021?  
    **Solution**:  
    P: 20,000 × 4 = $80,000. Q: 15,000 × 6 = $90,000. Ratio = 80,000 : 90,000 = 8 : 9.  
    **Answer**: 8 : 9

16. **Question**: Which product had higher cost growth per unit from 2021 to 2022?  
    **Solution**:  
    P: (5 - 4) ÷ 4 × 100 = 25%. Q: (7 - 6) ÷ 6 × 100 ≈ 16.67%. P is higher.  
    **Answer**: Product P

17. **Question**: What is the total units produced in 2022?  
    **Solution**:  
    P: 22,000 + Q: 18,000 = 40,000 units.  
    **Answer**: 40,000 units

18. **Question**: What is the percentage contribution of Product Q’s cost to total cost in 2023?  
    **Solution**:  
    Q: $160,000. Total: $310,000. % = (160,000 ÷ 310,000) × 100 ≈ 51.61%.  
    **Answer**: 51.61%

19. **Question**: What is the difference in production cost for Product P between 2021 and 2023?  
    **Solution**:  
    2021: 20,000 × 4 = $80,000. 2023: 25,000 × 6 = $150,000. Difference = 150,000 - 80,000 = $70,000.  
    **Answer**: $70,000

20. **Question**: What is the weighted average cost per unit in 2022, weighted by units produced?  
    **Solution**:  
    Total units = 40,000. Cost = (22,000 × 5) + (18,000 × 7) = 110,000 + 126,000 = $236,000.  
    Average = 236,000 ÷ 40,000 = $5.90.  
    **Answer**: $5.90

## Stacked Bar Graph-Based Questions (21–40)

**Stacked Bar Graph 1: Revenue ($1000) by Product Category in Three Cities (2021–2023)**  
- 2021: City A (Electronics: 300, Apparel: 200, Food: 100), City B (200, 150, 50), City C (250, 100, 50)  
- 2022: City A (350, 220, 120), City B (220, 160, 60), City C (270, 120, 60)  
- 2023: City A (400, 250, 150), City B (250, 180, 70), City C (300, 150, 80)

21. **Question**: What is the total revenue from Electronics in City A over the three years?  
    **Solution**:  
    Total = 300 + 350 + 400 = 1050 ($1000) = $1,050,000.  
    **Answer**: $1,050,000

22. **Question**: Which city had the highest Apparel revenue in 2023?  
    **Solution**:  
    A: 250, B: 180, C: 150. Highest is A.  
    **Answer**: City A

23. **Question**: What is the percentage growth of Food revenue in City B from 2021 to 2023?  
    **Solution**:  
    Increase = 70 - 50 = 20. % Growth = (20 ÷ 50) × 100 = 40%.  
    **Answer**: 40%

24. **Question**: What is the total revenue in City C in 2022?  
    **Solution**:  
    Total = 270 + 120 + 60 = 450 ($1000) = $450,000.  
    **Answer**: $450,000

25. **Question**: What is the ratio of Electronics to Apparel revenue in City A in 2021?  
    **Solution**:  
    Electronics (300) : Apparel (200) = 300 : 200 = 3 : 2.  
    **Answer**: 3 : 2

26. **Question**: Which category showed the highest growth in City C from 2021 to 2023?  
    **Solution**:  
    Electronics: (300 - 250) ÷ 250 × 100 = 20%.  
    Apparel: (150 - 100) ÷ 100 × 100 = 50%.  
    Food: (80 - 50) ÷ 50 × 100 = 60%.  
    Highest is Food.  
    **Answer**: Food

27. **Question**: What is the percentage contribution of Electronics to total revenue in City B in 2023?  
    **Solution**:  
    Total = 250 + 180 + 70 = 500. % Electronics = (250 ÷ 500) × 100 = 50%.  
    **Answer**: 50%

28. **Question**: What is the combined revenue of Apparel and Food in City A in 2022?  
    **Solution**:  
    Apparel (220) + Food (120) = 340 ($1000) = $340,000.  
    **Answer**: $340,000

29. **Question**: Which year had the highest total revenue across all cities?  
    **Solution**:  
    2021: A (600) + B (400) + C (400) = 1400.  
    2022: A (690) + B (440) + C (450) = 1580.  
    2023: A (800) + B (500) + C (530) = 1830 ($1000).  
    Highest is 2023.  
    **Answer**: 2023

30. **Question**: What is the CAGR of total revenue in City A from 2021 to 2023?  
    **Solution**:  
    Initial = 600, Final = 800. CAGR = [(800 ÷ 600)^(1/2) - 1] × 100 ≈ 15.47%.  
    **Answer**: 15.47%

**Stacked Bar Graph 2: Student Enrollments by Program (2021–2023)**  
- 2021: UG (500), PG (300), Diploma (200)  
- 2022: UG (550), PG (320), Diploma (220)  
- 2023: UG (600), PG (350), Diploma (250)

31. **Question**: What is the total enrollment in PG over the three years?  
    **Solution**:  
    Total = 300 + 320 + 350 = 970 students.  
    **Answer**: 970 students

32. **Question**: Which program had the highest enrollment in 2023?  
    **Solution**:  
    UG (600), PG (350), Diploma (250). Highest is UG.  
    **Answer**: UG

33. **Question**: What is the percentage growth of Diploma enrollment from 2021 to 2023?  
    **Solution**:  
    Increase = 250 - 200 = 50. % Growth = (50 ÷ 200) × 100 = 25%.  
    **Answer**: 25%

34. **Question**: What is the total enrollment in 2022?  
    **Solution**:  
    Total = 550 + 320 + 220 = 1090 students.  
    **Answer**: 1090 students

35. **Question**: What is the ratio of UG to PG enrollment in 2021?  
    **Solution**:  
    UG (500) : PG (300) = 500 : 300 = 5 : 3.  
    **Answer**: 5 : 3

36. **Question**: Which program showed the highest percentage growth from 2021 to 2022?  
    **Solution**:  
    UG: (550 - 500) ÷ 500 × 100 = 10%.  
    PG: (320 - 300) ÷ 300 × 100 ≈ 6.67%.  
    Diploma: (220 - 200) ÷ 200 × 100 = 10%.  
    UG and Diploma tie.  
    **Answer**: UG or Diploma

37. **Question**: What is the percentage contribution of PG to total enrollment in 2023?  
    **Solution**:  
    Total = 600 + 350 + 250 = 1200. % PG = (350 ÷ 1200) × 100 ≈ 29.17%.  
    **Answer**: 29.17%

38. **Question**: What is the combined enrollment of UG and Diploma in 2022?  
    **Solution**:  
    UG (550) + Diploma (220) = 770 students.  
    **Answer**: 770 students

39. **Question**: Which year had the highest total enrollment?  
    **Solution**:  
    2021: 1000. 2022: 1090. 2023: 1200. Highest is 2023.  
    **Answer**: 2023

40. **Question**: What is the CAGR of UG enrollment from 2021 to 2023?  
    **Solution**:  
    Initial = 500, Final = 600. CAGR = [(600 ÷ 500)^(1/2) - 1] × 100 ≈ 9.54%.  
    **Answer**: 9.54%

## Combination Chart-Based Questions (41–60)

**Combination Chart 1: Sales (units) and Profit Margin (%) of a Product (2019–2023)**  
- Bar (Sales): 2019 (10,000), 2020 (12,000), 2021 (15,000), 2022 (18,000), 2023 (20,000)  
- Line (Profit Margin): 2019 (5%), 2020 (6%), 2021 (7%), 2022 (8%), 2023 (10%)

41. **Question**: What is the profit in 2023?  
    **Solution**:  
    Profit = Sales × Margin = 20,000 × (10 ÷ 100) = 2000 units.  
    **Answer**: 2000 units

42. **Question**: Which year had the highest profit margin?  
    **Solution**:  
    2023 (10%) is highest.  
    **Answer**: 2023

43. **Question**: What is the CAGR of sales from 2019 to 2023?  
    **Solution**:  
    Initial = 10,000, Final = 20,000. CAGR = [(20,000 ÷ 10,000)^(1/4) - 1] × 100 ≈ 18.92%.  
    **Answer**: 18.92%

44. **Question**: What is the total profit over the five years?  
    **Solution**:  
    2019: 10,000 × 0.05 = 500. 2020: 12,000 × 0.06 = 720. 2021: 15,000 × 0.07 = 1050.  
    2022: 18,000 × 0.08 = 1440. 2023: 2000. Total = 500 + 720 + 1050 + 1440 + 2000 = 5710 units.  
    **Answer**: 5710 units

45. **Question**: What is the ratio of profit in 2021 to 2022?  
    **Solution**:  
    2021: 1050. 2022: 1440. Ratio = 1050 : 1440 = 7 : 9.6 ≈ 35 : 48.  
    **Answer**: 35 : 48

46. **Question**: Which year showed the highest percentage growth in sales?  
    **Solution**:  
    2020: (12,000 - 10,000) ÷ 10,000 × 100 = 20%.  
    2021: (15,000 - 12,000) ÷ 12,000 × 100 = 25%.  
    2022: (18,000 - 15,000) ÷ 15,000 × 100 = 20%.  
    2023: (20,000 - 18,000) ÷ 18,000 × 100 ≈ 11.11%.  
    Highest is 2021.  
    **Answer**: 2021

47. **Question**: What is the percentage contribution of 2023 profit to total profit?  
    **Solution**:  
    Total profit = 5710. 2023: 2000. % = (2000 ÷ 5710) × 100 ≈ 35.03%.  
    **Answer**: 35.03%

48. **Question**: What is the average profit margin over the five years?  
    **Solution**:  
    Total = 5 + 6 + 7 + 8 + 10 = 36. Average = 36 ÷ 5 = 7.2%.  
    **Answer**: 7.2%

49. **Question**: What is the difference in profit between 2022 and 2023?  
    **Solution**:  
    2023: 2000 - 2022: 1440 = 560 units.  
    **Answer**: 560 units

50. **Question**: If sales in 2024 are projected to grow by 10% with a 12% margin, what is the projected profit?  
    **Solution**:  
    2023 Sales = 20,000. 2024 Sales = 20,000 × 1.1 = 22,000. Profit = 22,000 × 0.12 = 2640 units.  
    **Answer**: 2640 units

**Combination Chart 2: Revenue ($1000) and Growth Rate (%) of a Company (2020–2023)**  
- Bar (Revenue): 2020 (500), 2021 (600), 2022 (750), 2023 (900)  
- Line (Growth Rate): 2021 (20%), 2022 (25%), 2023 (20%)

51. **Question**: What is the revenue in 2023?  
    **Solution**:  
    Revenue = 900 ($1000) = $900,000.  
    **Answer**: $900,000

52. **Question**: Which year had the highest growth rate?  
    **Solution**:  
    2022 (25%) is highest.  
    **Answer**: 2022

53. **Question**: What is the CAGR of revenue from 2020 to 2023?  
    **Solution**:  
    Initial = 500, Final = 900. CAGR = [(900 ÷ 500)^(1/3) - 1] × 100 ≈ 21.64%.  
    **Answer**: 21.64%

54. **Question**: What is the total revenue over the four years?  
    **Solution**:  
    Total = 500 + 600 + 750 + 900 = 2750 ($1000) = $2,750,000.  
    **Answer**: $2,750,000

55. **Question**: What is the ratio of revenue in 2021 to 2022?  
    **Solution**:  
    2021 (600) : 2022 (750) = 600 : 750 = 4 : 5.  
    **Answer**: 4 : 5

56. **Question**: What is the absolute growth in revenue from 2020 to 2023?  
    **Solution**:  
    Growth = 900 - 500 = 400 ($1000) = $400,000.  
    **Answer**: $400,000

57. **Question**: What is the percentage contribution of 2022 revenue to total revenue?  
    **Solution**:  
    2022: 750. Total: 2750. % = (750 ÷ 2750) × 100 ≈ 27.27%.  
    **Answer**: 27.27%

58. **Question**: What is the average growth rate from 2021 to 2023?  
    **Solution**:  
    Total = 20 + 25 + 20 = 65. Average = 65 ÷ 3 ≈ 21.67%.  
    **Answer**: 21.67%

59. **Question**: What is the difference in revenue between 2022 and 2023?  
    **Solution**:  
    2023: 900 - 2022: 750 = 150 ($1000) = $150,000.  
    **Answer**: $150,000

60. **Question**: If 2024 revenue grows at 15%, what is the projected revenue?  
    **Solution**:  
    2023: 900. 2024 = 900 × 1.15 = 1035 ($1000) = $1,035,000.  
    **Answer**: $1,035,000

## Pie Chart with Secondary Data-Based Questions (61–80)

**Pie Chart 1: Market Share (%) and Revenue ($1000) of Four Companies in 2023**  
- Company A: 40%, Revenue: 800  
- Company B: 30%, Revenue: 600  
- Company C: 20%, Revenue: 400  
- Company D: 10%, Revenue: 200  

61. **Question**: What is the total market revenue in 2023?  
    **Solution**:  
    Total = 800 + 600 + 400 + 200 = 2000 ($1000) = $2,000,000.  
    **Answer**: $2,000,000

62. **Question**: Which company has the highest market share?  
    **Solution**:  
    A (40%) is highest.  
    **Answer**: Company A

63. **Question**: What is the ratio of revenue of Company A to Company C?  
    **Solution**:  
    A (800) : C (400) = 800 : 400 = 2 : 1.  
    **Answer**: 2 : 1

64. **Question**: What is the percentage contribution of Company B’s revenue to total revenue?  
    **Solution**:  
    B: 600. Total: 2000. % = (600 ÷ 2000) × 100 = 30%.  
    **Answer**: 30%

65. **Question**: If Company D’s revenue grows by 25% in 2024, what is the new revenue?  
    **Solution**:  
    D: 200. Increase = 200 × 0.25 = 50. New = 200 + 50 = 250 ($1000) = $250,000.  
    **Answer**: $250,000

66. **Question**: What is the combined market share of Companies C and D?  
    **Solution**:  
    C (20%) + D (10%) = 30%.  
    **Answer**: 30%

67. **Question**: What is the difference in revenue between Companies A and B?  
    **Solution**:  
    A (800) - B (600) = 200 ($1000) = $200,000.  
    **Answer**: $200,000

68. **Question**: If total market revenue grows by 10% in 2024, what is Company A’s projected revenue (same share)?  
    **Solution**:  
    Total: 2000 × 1.1 = 2200. A: 40% of 2200 = 880 ($1000) = $880,000.  
    **Answer**: $880,000

69. **Question**: What is the weighted average market share, weighted by revenue?  
    **Solution**:  
    Weighted share = [(40 × 800) + (30 × 600) + (20 × 400) + (10 × 200)] ÷ 2000 = 40%.  
    **Answer**: 40%

70. **Question**: Which company has the lowest revenue?  
    **Solution**:  
    D (200) is lowest.  
    **Answer**: Company D

**Pie Chart 2: Budget Allocation (%) and Actual Spending ($1000) in 2023**  
- Salaries: 50%, Spending: 1000  
- Rent: 20%, Spending: 400  
- Supplies: 15%, Spending: 300  
- Marketing: 15%, Spending: 300  

71. **Question**: What is the total budget spending in 2023?  
    **Solution**:  
    Total = 1000 + 400 + 300 + 300 = 2000 ($1000) = $2,000,000.  
    **Answer**: $2,000,000

72. **Question**: Which category has the highest allocation?  
    **Solution**:  
    Salaries (50%) is highest.  
    **Answer**: Salaries

73. **Question**: What is the ratio of Salaries to Rent spending?  
    **Solution**:  
    Salaries (1000) : Rent (400) = 1000 : 400 = 5 : 2.  
    **Answer**: 5 : 2

74. **Question**: What is the percentage contribution of Supplies to total spending?  
    **Solution**:  
    Supplies: 300. Total: 2000. % = (300 ÷ 2000) × 100 = 15%.  
    **Answer**: 15%

75. **Question**: If Marketing spending increases by 20% in 2024, what is the new amount?  
    **Solution**:  
    Marketing: 300. Increase = 300 × 0.2 = 60. New = 300 + 60 = 360 ($1000) = $360,000.  
    **Answer**: $360,000

76. **Question**: What is the combined allocation of Rent and Supplies?  
    **Solution**:  
    Rent (20%) + Supplies (15%) = 35%.  
    **Answer**: 35%

77. **Question**: What is the difference in spending between Salaries and Marketing?  
    **Solution**:  
    Salaries (1000) - Marketing (300) = 700 ($1000) = $700,000.  
    **Answer**: $700,000

78. **Question**: If total spending grows by 5% in 2024, what is Salaries’ projected spending (same allocation)?  
    **Solution**:  
    Total: 2000 × 1.05 = 2100. Salaries: 50% of 2100 = 1050 ($1000) = $1,050,000.  
    **Answer**: $1,050,000

79. **Question**: What is the weighted average allocation, weighted by spending?  
    **Solution**:  
    Weighted = [(50 × 1000) + (20 × 400) + (15 × 300) + (15 × 300)] ÷ 2000 = 50%.  
    **Answer**: 50%

80. **Question**: Which categories have equal spending?  
    **Solution**:  
    Supplies (300) and Marketing (300) are equal.  
    **Answer**: Supplies and Marketing

## Caselet-Based Questions (81–100)

**Caselet 1: A Retail Chain’s Sales and Costs**  
- Store A: 1000 units sold at $50/unit, 10% discount, cost $30/unit  
- Store B: 800 units sold at $60/unit, 15% discount, cost $35/unit  
- Store C: 600 units sold at $70/unit, no discount, cost $40/unit  

81. **Question**: What is the revenue from Store A after discount?  
    **Solution**:  
    Discount = 10% of 50 = 5. Price = 50 - 5 = 45. Revenue = 1000 × 45 = $45,000.  
    **Answer**: $45,000

82. **Question**: What is the profit from Store B?  
    **Solution**:  
    Discount = 15% of 60 = 9. Price = 60 - 9 = 51. Revenue = 800 × 51 = $40,800.  
    Cost = 800 × 35 = $28,000. Profit = 40,800 - 28,000 = $12,800.  
    **Answer**: $12,800

83. **Question**: What is the total revenue from all stores?  
    **Solution**:  
    A: $45,000. B: $40,800. C: 600 × 70 = $42,000. Total = 45,000 + 40,800 + 42,000 = $127,800.  
    **Answer**: $127,800

84. **Question**: What is the total profit margin (%) across all stores?  
    **Solution**:  
    Total cost: A: 1000 × 30 = 30,000. B: 28,000. C: 600 × 40 = 24,000. Total = 82,000.  
    Profit = 127,800 - 82,000 = 45,800. Margin = (45,800 ÷ 127,800) × 100 ≈ 35.84%.  
    **Answer**: 35.84%

85. **Question**: Which store has the highest profit?  
    **Solution**:  
    A: 45,000 - 30,000 = $15,000. B: $12,800. C: 42,000 - 24,000 = $18,000. Highest is C.  
    **Answer**: Store C

86. **Question**: What is the weighted average selling price per unit after discounts?  
    **Solution**:  
    Total units = 1000 + 800 + 600 = 2400. Revenue = $127,800. Average = 127,800 ÷ 2400 = $53.25.  
    **Answer**: $53.25

87. **Question**: What is the ratio of units sold in Store A to Store C?  
    **Solution**:  
    A (1000) : C (600) = 1000 : 600 = 5 : 3.  
    **Answer**: 5 : 3

88. **Question**: What is the percentage contribution of Store B’s profit to total profit?  
    **Solution**:  
    Total profit = 45,800. B: 12,800. % = (12,800 ÷ 45,800) × 100 ≈ 27.95%.  
    **Answer**: 27.95%

89. **Question**: What is the total discount amount across all stores?  
    **Solution**:  
    A: 1000 × 5 = $5000. B: 800 × 9 = $7200. C: $0. Total = 5000 + 7200 = $12,200.  
    **Answer**: $12,200

90. **Question**: If Store C’s units sold increase by 20%, what is the new profit?  
    **Solution**:  
    New units = 600 × 1.2 = 720. Revenue = 720 × 70 = $50,400. Cost = 720 × 40 = $28,800.  
    Profit = 50,400 - 28,800 = $21,600.  
    **Answer**: $21,600

**Caselet 2: A University’s Research Funding and Publications**  
- Dept A: $500,000 funding, 50 publications, 20% high-impact  
- Dept B: $400,000 funding, 40 publications, 25% high-impact  
- Dept C: $300,000 funding, 30 publications, 30% high-impact  

91. **Question**: How many high-impact publications did Dept A produce?  
    **Solution**:  
    High-impact = 20% of 50 = 10 publications.  
    **Answer**: 10 publications

92. **Question**: What is the average funding per publication for Dept B?  
    **Solution**:  
    Funding = $400,000. Publications = 40. Average = 400,000 ÷ 40 = $10,000.  
    **Answer**: $10,000

93. **Question**: Which department had the highest number of high-impact publications?  
    **Solution**:  
    A: 10. B: 25% of 40 = 10. C: 30% of 30 = 9. A and B tie.  
    **Answer**: Dept A or B

94. **Question**: What is the total funding across all departments?  
    **Solution**:  
    Total = 500,000 + 400,000 + 300,000 = $1,200,000.  
    **Answer**: $1,200,000

95. **Question**: What is the total number of publications across all departments?  
    **Solution**:  
    Total = 50 + 40 + 30 = 120 publications.  
    **Answer**: 120 publications

96. **Question**: What is the weighted average funding per publication?  
    **Solution**:  
    Total funding = $1,200,000. Total publications = 120. Average = 1,200,000 ÷ 120 = $10,000.  
    **Answer**: $10,000

97. **Question**: What is the ratio of high-impact publications in Dept B to Dept C?  
    **Solution**:  
    B: 10. C: 9. Ratio = 10 : 9.  
    **Answer**: 10 : 9

98. **Question**: What is the percentage contribution of Dept C’s funding to total funding?  
    **Solution**:  
    C: 300,000. Total: 1,200,000. % = (300,000 ÷ 1,200,000) × 100 = 25%.  
    **Answer**: 25%

99. **Question**: What is the total number of high-impact publications?  
    **Solution**:  
    A: 10, B: 10, C: 9. Total = 10 + 10 + 9 = 29.  
    **Answer**: 29 publications

100. **Question**: If Dept A’s funding increases by 10% and publications remain the same, what is the new funding per publication?  
     **Solution**:  
     New funding = 500,000 × 1.1 = $550,000. Publications = 50. Average = 550,000 ÷ 50 = $11,000.  
     **Answer**: $11,000