# Stock_Algorithms_Pseudo
ALGORITHMS AND DATA STRUCTURES
Project 4									Pham Hoang Son

Develop an algorithms to rate a stock potential.
Disclaimer: the algorithm I developed is based on past stock information and data. There are many more factors that affect stock prices that we cannot predict with algorithms.


1.	Alternative Structures:
START
float current_price, high, low;

 current_price = input("Enter current price: "); // Input current price, 52-week high, and 52-week low  
high = input("Enter 52-week high: ")
low = input("Enter 52-week low: ")

if (current_price > high) {
    output("Sell")
} else if (current_price < low) {
    output("Buy")
} else {
    output("Hold")
}
END
The 52-week high/low is the highest and lowest price at which a security has traded during the time period that equates to one year and is viewed as a technical indicator. In order to avoid risky stock that might be disappear in the future from the stock market.
2. Repetitive Structures:
START
float current_price, avg_price, num_days;
 current_price = input("Enter current price: ");
num_days = input("Enter number of days: ");
 
float sum = 0;
 for (int i = 0; i < num_days; i++) {
    float price = input("Enter price for day " + i + ": ");
    sum += price;
}
avg_price = sum / num_days;
 while (current_price < avg_price) {
    output("Buy");
    current_price = input("Enter current price: ");
}
output("Sell");
END
By using loop functions to calculate sums of the price in how many days that we want to calculate through input value. After we find our average price through input data, then we can compare the current price with the average price to decide for ourselves.
3.  One-Dimensional Array Processing:
START
float prices[N];       // Initialize array for past 10 closing prices
for (int i = 0; i < 10; i++) {
    prices[i] = input("Enter closing price for day " + i + ": ");
}
 float sum = 0;      // Initialize variable for sum of prices
 
for (int i = 0; i < 10; i++) {      // Use for loop to sum prices  
    sum += prices[i];
}
float avg_price = sum / 10;
 
if (prices[10] > avg_price) {
    output("Buy");
} else {
    output("Sell");
}
END
By using if statement, we can determine whether to buy it or sell the stock.
4. Two-Dimensional Array Processing:
START
Float avgPreviousPrice[10];
For (int i = 0; I < 10; i++) {
avgPreviousPrice[I] = input(“Enter the last ten day price” + i +  “:”);
}
Float sum = 0;
for (int i = 0; i < 10; i++) {      
    sum += prices[i];
}
float avgPreviousPrice = sum / 10;
 
float prices[10][3];
 
for (int i = 0; i < 10; i++) {
    prices[i][0] = input("Enter open price for day " + i + ": ");  //INPUT for open price
    prices[i][1] = input("Enter high price for day " + i + ": ");   //INPUT for high price
    prices[i][2] = input(“Enter low price for day “ + j + “: ”);    //INPUT for low price
For I = 0 to 30
IF prices > avgPrice:
FOR I TO X:
PRINT I
PRINT( ‘Total prices are greater than average day is :  ‘   ,i  )
ELSE :
FALSE
END

 
float array1[10], array2[10], array3[10], sumArray[30];
 
for (int i = 0; i < 10; i++) {
    sumArray[i] = array1[i] + array2[i] + array3[i];
}
float avgPrice = sum / 30;
if (avgPreviousPrice[10] > avgPrice) {
    output("Buy");
} else {
    output("Sell");
}
END
By using loop functions to calculate average price of last 10 previous days, then we could compare it with our current today price and make a decision to buy it or sell it






