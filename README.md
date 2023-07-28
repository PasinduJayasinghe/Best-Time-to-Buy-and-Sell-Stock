# Best-Time-to-Buy-and-Sell-Stock

## Description
This is a solution for the LeetCode problem known as "Best Time to Buy and Sell Stock" problem. The problem includes searching through array to find a suitable day to sell a stock. 

## Goal of the Project
My goal is to provide solutions for the problems in LeetCode using documentation and providing code. First, I will complete this project for the NeetCode's 75 LeetCode problems. 
The documentation of the problem generated using ChatGPT. But I reviewed it before publishing here.

## maxProfit(self, prices: List[int]) -> int
This function is a method of the Solution class. It aims to find the maximum profit that can be obtained from a list of stock prices. The function takes a list of integers (prices) as input and returns an integer, which represents the maximum profit.

### Parameters:
prices (List[int]): A list of integers representing the stock prices for different days. 
max_profit (int): An integer representing the maximum profit that can be obtained by buying and selling the stock at the right moments.

### Algorithm:
Initialize two pointers, l and r, with values 0 and 1, respectively. These pointers represent the left and right indices of a sliding window that will be used to find potential profit opportunities in the stock prices list.
Initialize the max_profit variable to 0. This will store the maximum profit found so far.
Start a while loop that runs until the right pointer r reaches the end of the prices list.
Inside the loop, check if the stock price at index l (prices[l]) is less than the stock price at index r (prices[r]). If this condition is true, it indicates a potential profit opportunity.
Calculate the profit as the difference between the stock prices at indices r and l (prices[r] - prices[l]).
Update the max_profit to store the maximum value between the current max_profit and the calculated profit using the max function.
If the stock price at index l is greater than or equal to the stock price at index r, there is no potential profit between these two indices. In this case, update l to the current r value. This effectively moves the left pointer to the right to start a new potential profit window.
Increment the right pointer r to move the window to the right for the next iteration.
Continue the loop until r reaches the end of the prices list.
Once the loop ends, the max_profit variable will hold the maximum profit that can be obtained from the given list of stock prices. Return the value of max_profit as the output of the function.

### problem Link
https://leetcode.com/problems/two-sum/
### NeetCode Problems List
https://docs.google.com/spreadsheets/d/1A2PaQKcdwO_lwxz9bAnxXnIQayCouZP6d-ENrBz_NXc/edit#gid=0
