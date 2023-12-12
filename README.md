## UserStory

As a software developer I have to create a program that is analyzing the financial records of a company.

## AcceptanceCriteria

- It is done when when the total number of months included in the dataset.

- It is done when the net total amount of Profit/Losses over the entire period.

- It is done when the average of the changes in Profit/Losses over the entire period.

- It is done when You will need to track what the total change in Profit/Losses are from month to month and then find the average. (Total/(Number of months - 1))

- It is done when the greatest increase in Profit/Losses (date and amount) over the entire period.

- It is done when the greatest decrease in Profit/Losses (date and amount) over the entire period.

## PseudoCode

// You have been given a dataset composed of arrays with two fields, Date and Profit / Losses.

// Your task is to write JavaScript code that analyzes the records to calculate each of the following:

// The total number of months included in the dataset.
// finances.length

// The net total amount of Profit / Losses over the entire period.
// Need a variable for Profits/Losses
// Need to be able to compare the data for the loop that we're on to the data from the previous loop
// Need variables for current & previous once we start the loop
// Need an if statement to make sure we're on at least month 2 (array index 1) before starting to figure profits & losses

// The average of the changes in Profit / Losses over the entire period.
// -Need a variable to track the average change
// -That will make use of the current & previous variables we set up before
// -You will need to track what the total change in Profit / Losses are from month to month and then find the average.
// (Total / (Number of months - 1))

// The greatest increase in Profit / Losses(date and amount) over the entire period.
// -Need a variable for the greatest increase
// -On each iteration, compare the current change in profits/losses to what's currently stored
// -If the change is more, replace what's currently stored in the variable

// The greatest decrease in Profit / Losses(date and amount) over the entire period.
// - Need a variable for the greatest decrease
// - On each iteration, compare the current change in profits/losses to what's currently stored
// - If the loss is greater, replace what's currently stored in the variable

// variables:
// total number of months
// rolling total of profits
// greatest increase (month & amt)
// greatest loss (month & amt)
// average of the changes

// variables declared inside the loop:
// current data point
// previous data point

## Solution

- I have startred the challange by frist creating the pseudocode. The problem has been broken down into
  small steps in order to ease down the process of solving it.

- The next step was to declera variable so later I can use them to store the the solution values.

- I have used a for loop to iterate through the finances array: inside the loop I have frist calculates the totalProfitLoss by summing up all the profit/loss amounts, then I have calculated the change in profit/loss between the current and previous months, updates the totalDifference variable with this difference, and tracks the greatest increase and decrease.

- The next step was calculating the average change in profit or loss per interval between consecutive months in the data.
