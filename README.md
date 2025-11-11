# Tax-Slab
Write a program to calculate the total income tax paid in old and new tax slabs by taking the annual salary from the user.  Old Tax Slab:  Annual Salary (Rs.)  Income Tax Rates  0 to 250000  Nil  250000 to 500000  5%  500000 to 1000000  20%  Greater than 1000000  30%  Note: The olda Tax slab has rebate if the annual salary is &lt;= 500000.

Explanation of the Logic
The program uses a sequential if-else if structure, which ensures that the conditions are checked in order. 
The program first checks if the salary is within the first slab (up to 2,50,000). If it is, the tax is 0.
If not, it moves to the next else if and checks if the salary is up to 5,00,000. Because the first condition was false, the code here only runs for the amount above 2,50,000. It calculates 5% of that difference.
This pattern continues, with each block calculating the tax only on the portion of income that falls within that specific bracket, and adding it to the base tax amount from previous brackets.
The final else block catches any income that is higher than the last defined slab. 
