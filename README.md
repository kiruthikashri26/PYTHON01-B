Exp-no---1B--Product-Price-Analysis-Using-Python-Functions




Aim:



To analyze quarterly sales data using NumPy arrays.



Algorithm:



1. Import NumPy.


2. Create 2D array (rows = products, columns = quarters).


3. Calculate total and average sales per product and per quarter.


4. Display summary.





Program:



     import numpy as np

sales = np.array([[1000, 1200, 1150, 1400],
                  [800, 950, 1050, 1300],
                  [1500, 1600, 1550, 1700]])

print("Sales Data (Rows=Products, Columns=Quarters):\n", sales)



product_total = np.sum(sales, axis=1)



quarter_total = np.sum(sales, axis=0)



overall_avg = np.mean(sales)



print("\nTotal Sales per Product:", product_total)



print("Total Sales per Quarter:", quarter_total)



print("Overall Average Sales:", overall_avg)



print("Highest Sale:", np.max(sales))



print("Lowest Sale:", np.min(sales))



Output:


Sales Data (Rows=Products, Columns=Quarters):


[[1000 1200 1150 1400]
 [ 800  950 1050 1300]
 [1500 1600 1550 1700]]

Total Sales per Product: [4750 4100 6350]


Total Sales per Quarter: [3300 3750 3750 4400]


Overall Average Sales: 1266.6666666666667



Highest Sale: 1700


Lowest Sale: 800





Result:


The program successfully analyzes quarterly product sales using NumPy arrays and Python functions.
