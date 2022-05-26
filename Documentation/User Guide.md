# User Guide

This User Guide explains how to use the Expense Management Spreadsheet to manage expenses, savings, and inventory.

## Contents

[Expense Estimate](#Expense-Estimate)

[Day-off Spending](#Day-off-Spending)

[Inventory](#Inventory)

[Monthly Expense Calculator](#Monthly-Expense-Calculator)

[Fund Management Tool](#Fund-Management-Tool)

## Expense Estimate

Some expenses are regular in our daily lives and can be estimated by assumptions and calculations. In this section, you will learn how to use the **Daily Expense** and **Subscription** tables to estimate your regular monthly expenses.

### Daily Expense Table

The Daily Expense table helps you estimate how much money you would spend each day. You can input the amount of money you would spend in maximum on weekdays and weekends for each category in the table. Here is what the Daily Expense Table looks like:

| Categories     | Each day expense in weekday | Total in weekday | Each day expense in weekend | Total in weekend | Total in 28 days | extra   | Total in categories |
| -------------- | --------------------------- | ---------------- | --------------------------- | ---------------- | ---------------- | ------- | ------------------- |
| Food           | \$100.00                     | \$500.00          | \$100.00                     | \$200.00          | \$2,800.00        | \$300.00 | \$3,100.00           |
| Transportation | \$40.00                      | \$200.00          | \$40.00                      | \$80.00           | \$1,120.00        | \$120.00 | \$1,240.00           |

There are multiple items on the table, each serves a different purpose:

- **Categories** - Name for the type of items you would spend money on (e.g. Food, transportation...)
- **Each day expense in weekday** - Estimated (maximum) amount of spending for the particular category on each day on weekdays
- **Total in weekday** - Based on the above input, the total amount of spending for the particular category on weekdays of a week (i.e. Monday to Friday) is calculated automatically
- **Each day expense in weekend** - Estimated (maximum) amount of spending for the particular category on each day on weekends
- **Total in weekend** - Based on the above input, the total amount of spending for the particular category on weekends of a week (i.e. Saturday and Sunday) is calculated automatically
- **Total in 28 days** - Based on the result in "Total in weekday" and "Total in weekend", automatically calculate the total amount of spending for the particular category in 4 weeks (i.e. 28 days)
- **extra** - Automatically calculate the total amount of spending of the remaining 3 days in a month for the particular category, based on the input in "Each day expense in weekend" (assuming every month has 31 days)
- **Total in categories** - equal to the sum of value in "Total in 28 days" and "extra"

### Subscription Table

Subscriptions are another type of expense that is consistent throughout every month. The Subscription table helps you record services that you have to pay monthly/yearly subscriptions for. Here is what the Subscription table looks like:

| Services / Regular Expense | Charge period | Price   | Monthly Price |
| -------------------------- | ------------- | ------- | ------------- |
| Month  Subscription 1      | Monthly       | \$68.00  | \$68.00       |
| Yearly  Subscription 1     | Yearly        | \$680.00 | \$56.67       |

There are multiple items on the table, each serves a different purpose:

- **Services / Regular Expenses** - Name of the service that you have subscribed to
- **Charge period** - The frequency of the payment for the service. It can be `Monthly` (i.e. You would be charged every month) or `Yearly` (i.e. You would be charged every year)
- **Price** - The (monthly / yearly) price of the service
- **Monthly Price** - If you choose `Monthly` for the "Charge period", the "Monthly Price" is the same as your input in "Price"; Else, if you choose `Yearly`, the "Monthly Price" would be the input in "Price" divided by 12 (i.e. The average price you have to pay in every month)

### Three tiers for Expense Estimate

There are three tiers for estimating your expenses so that you can select one for expense calculation, based on your current financial situation. The three tiers are as below:

- **Original** (`Expense Estimate (Daily)` and `Expense Estimate (Subscription)` sheets)

  This mode is for estimating your "usual" spending pattern and there is no need to reduce your expense to cater to some special situation.

- **Lower Budget Mode** (`Lower Budget Mode (Daily)` and `Lower Budget Mode (Subscription` sheets)

  This mode is for when you would like to reduce your expenses a little bit, but it is not necessary to reduce your expense to your absolute minimum.

- **Minimum Expense** (`Minimum Expense (Daily)` and `Minimum Expense (Subscription)` sheets)

	This mode is for when you feel like you need to reduce your expense to the absolute minimum.

Once you have finished estimating your expense for all three tiers, you can see the total amount of monthly expenses for each mode and compare the amount between them, by going to the "Expense comparison" sheet.

![image-20220526105834273](User%20Guide.assets/image-20220526105834273.png)

## Day-off Spending

Day-off Spending sheet is for recording the expenses on day-offs, which are usually higher than the regular (estimated) expenses. The spending on day-offs can be categorized into different types and the table for recording day-off expenses is as below:

| Date     | Public Transport | Taxi/Uber | Food and Snacks | Drink   | Total Spending |
| -------- | ---------------- | --------- | --------------- | ------- | -------------- |
| 1/8/2021 | \$60.00          | \$200.00  | \$150.00        | \$50.00 | \$460.00       |
| 8/8/2021 | \$40.00          | \$0.00    | \$100.00        | \$20.00 | \$160.00       |
| 1/9/2021 | \$50.00          | \$0.00    | \$125.00        | \$30.00 | \$205.00       |
| 8/9/2021 | \$30.00          | \$150.00  | \$75.00         | \$10.00 | \$265.00       |

There are multiple items on the table, each serves a different purpose:

- **Date** - The date of the record
- **Public Transport** - Amount of money spent on public transportations on that day
- **Taxi/Uber** - Amount of money spent on Taxi/Uber on that day
- **Food and Snacks** - Amount of money spent on food and snacks on that day
- **Drink** - Amount of money spent on drinks
- **Total Spending** - The sum of spending in the above categories

Based on the entries in the table, the spreadsheet would calculate and display the statistics for your spending, including:

**Average Spending for All the Records**

![image-20220526193938699](User%20Guide.assets/image-20220526193938699.png)

Take all the entries in the Day-off Spending table and show the average amount of spending for each category.

**Average Spending and Total Spending for Date Range**

![image-20220526194030425](User%20Guide.assets/image-20220526194030425.png)

Take all the entries that meet the inputted date range (from `[The first date]` to `[The second date]`) in the Day-off Spending table and show the average and total amount of spending for each category, as well as the total spending (Sum of spending in all categories) in the date range.

![image-20220526194145313](User%20Guide.assets/image-20220526194145313.png)

Based on the result for total spending, a Pie Chart that visualizes the ratio of spending in each category among the total spending is shown.

**Total Spending of Different Months**

![image-20220526194122945](User%20Guide.assets/image-20220526194122945.png)

Show the total amount of spending for each month, and display a Line Chart that visualizes the changes in the total amount of spending for each month.

## Inventory

The inventory section is for recording the information of the items you have bought and the items you have replaced (obsoleted). In this section, you would learn how to use the **Inventory** and **Obsoleted Items** tables to record information about your bought items.

### Inventory Table

The Inventory table records the information of the items you currently have. Here is what the Inventory table looks like:

| Price      | Total day of ownership | Brand | Item Name | Date of buying | Warranty | (Useless Field) | Serial No | Notes |
| ---------- | ---------------------- | ----- | --------- | -------------- | -------- | --------------- | --------- | ----- |
| \$5,000.00 | 876.00                 | N.A.  | Laptop    | 1/1/2020       | 2 Year   |                 | N.A.      |       |
| \$3,000.00 | 845.00                 | N.A.  | Phone     | 1/2/2020       | 1 Year   |                 | N.A.      |       |
| \$200.00   | 298.00                 | N.A.  | Clothings | 1/8/2021       | N.A.     |                 | N.A.      |       |

There are multiple items on the table, each serves a different purpose:

- **Price** - The price of the item you bought
- **Total day of ownership** - The total number of day you owned the item, as of now (based on your System date and your input in "Date of buying")
- **Brand** - The brand of your item
- **Item Name** - The name (or the model) of your item
- **Date of buying** - The day you purchased the item
- **Warranty** - The warranty information for your item
- **(Useless Field)** - It is useless, as the name suggested. This field is originally intended for another purpose and now it is not used, but it is kept to ensure the calculation in `Inventory (Stat)` sheet works as expected.
- **Serial No** - Serial Number (if available) of your item
- **Notes** - Additional notes for your record, if any

### Obsoleted Items Table

The Obsoleted Items table records the information of the items you no longer want / own (i.e. it is "obsoleted"). Here is what the Obsoleted Items table looks like:

| Price      | No. of day owned | Brand | Item Name       | Date of buying | Date of obsolete | Notes                |
| ---------- | ---------------- | ----- | --------------- | -------------- | ---------------- | -------------------- |
| \$3,000.00 | 1826.00          | N.A.  | Custom Build PC | 1/1/2015       | 1/1/2020         | Sold to someone else |

There are multiple items on the table, each serves a different purpose:

- **Price** - The price of the item you bought
- **No. of day owned** - The total number of days you owned the item, based on your input in "Date of buying" and "Date of obsolete")
- **Brand** - The brand of your item
- **Item Name** - The name (or the model) of your item
- **Date of buying** - The day you purchased the item
- **Date of obsolete** - The day you no longer want/own the item (i.e. The item is "obsoleted")
- **Notes** - Additional notes for your record, if any

### Inventory (Statistics)

Based on your entries in the Inventory table and the Obsoleted Items table, the statistics of the item you owned (and you no longer owned) is shown on the `Inventory (Stat)` sheet:

![image-20220526195720453](User%20Guide.assets/image-20220526195720453.png)

There are multiple items shown in this sheet, including:

- **Total value** - The sum of the price of the items you currently owned
- **Most Expensive** - Top 3 most expensive items that you currently owned
- **Cheapest** - Top 3 cheapest items that you currently owned
- **(Top 3) Longest Ownership (Day)** - Top 3 items that you owned the longest time (in terms of day)
- **Most Occurred Brand** - The most frequently occurred Brand among all the items you currently owned
- **Obsoleted items - Longest Ownership (Day)** - Top 3 items you no longer want/owned that you owned the longest time (in terms of day)

## Monthly Expense Calculator

The total expense for the specified month is calculated based on the spending in different categories and your input.

![image-20220526195125691](User%20Guide.assets/image-20220526195125691.png)

There are multiple items shown in this sheet, including:

- **Year + Month (Manual input)** - Input the year and month that you would like to calculate the monthly expense for
- **Select Expense Mode** - Select one of the three modes for Expense Estimate. To switch to another mode, click on the **\[▾\]** button next to the name of the mode, then click on the mode you would like to select.

![image-20220526195209893](User%20Guide.assets/image-20220526195209893.png)

- **Essential Expense (excl. Day-off)** - Based on the mode you selected, the total amount of regular expenses (Including daily expenses and subscriptions) would be calculated. At the same time, based on the number of entries for day-offs that is within the specified year and month, the total amount of regular expenses would be subtracted by "the sum of spending in all categories in one weekend day" times "number of day-offs in the specified month"
- **Day-off Spending** - The sum of the money spent on day-offs within the specified year and month
- **Item purchased this month** - The sum of the price of the items that have the purchase date within the specified year month
- **Others (Manual input)** - Manually input the amount of money spent that is not recorded in the above categories
- **Total** - Sum of the money spent in the above categories

## Fund Management Tool

Fund Management Tool is a simple tool that helps you record savings for different purposes. In this section, you would learn how to use the Fund Management Tool to add, modify and remove funds (i.e. saving for different purposes).

To launch Fund Management Tool, go to the `Extra Tools` sheet and click on the `Fund Management Tool` button:

![image-20220526212720882](User%20Guide.assets/image-20220526212720882.png)

> **FYI:** on this page, there is also the "Last update" information which shows the time and date of the most recent time you saved the changes to the spreadsheet.

The Fund Management form would be shown:

![image-20220526212920717](User%20Guide.assets/image-20220526212920717.png)

### Add a new Fund

To add a new fund, press the **\[ADD\]** button. You would be prompted to enter a name for your new fund:

![image-20220526213244523](User%20Guide.assets/image-20220526213244523.png)

Enter the name of your new fund and press **\[OK\]**:

![image-20220526213642107](User%20Guide.assets/image-20220526213642107.png)

The new fund is already added to the list of funds and its balance is initialized to 0.

![image-20220526213720363](User%20Guide.assets/image-20220526213720363.png)

You can also enter the description of the fund (e.g. its purpose) at the text box below "Description:".

![image-20220526213921195](User%20Guide.assets/image-20220526213921195.png)

### Switch Between Funds

If you have more than one fund and you want to switch between them, you can do so by simply clicking the name of the fund you would like to switch to in the list below "Select Fund:".

![image-20220526214101804](User%20Guide.assets/image-20220526214101804.png)

The interface would display the information of your selected fund, including its name, its balance, and its description.

### Deposit to / Withdraw from the Fund

<u>Deposit Money to the Fund</u>

To deposit money into your selected fund, click the **\[DEPOSIT\]** button next to the balance.

![image-20220526214259731](User%20Guide.assets/image-20220526214259731.png)

You would be prompted to enter the amount you would like to deposit to the fund:

![image-20220526214616182](User%20Guide.assets/image-20220526214616182.png)

Enter the amount you would like to deposit and press **\[OK\]**:

![image-20220526214641859](User%20Guide.assets/image-20220526214641859.png)

The entered amount would be added to your original balance of the selected fund and the new balance would be shown:

![image-20220526214801845](User%20Guide.assets/image-20220526214801845.png)

<u>Withdraw Money from the Fund</u>

To withdraw money from the fund, click the **\[WITHDRAW\]** button next to the balance. You would be prompted to enter the amount you would like to withdraw from the fund:

![image-20220526214945085](User%20Guide.assets/image-20220526214945085.png)

Enter the amount you would like to withdraw and press **\[OK\]**:

![image-20220526215018122](User%20Guide.assets/image-20220526215018122.png)

The entered amount would be deducted from your original balance of the selected fund and the new balance would be shown:

![image-20220526215043066](User%20Guide.assets/image-20220526215043066.png)

### Rename a Fund

To give a new name for a fund, press the **\[RENAME FUND\]** button below the list of funds. You would be prompted to enter a new name for the fund:

![image-20220526215243785](User%20Guide.assets/image-20220526215243785.png)

Enter a new name of your fund and press **\[OK\]**:

![image-20220526215356108](User%20Guide.assets/image-20220526215356108.png)

The name of your fund is now changed:

![image-20220526215441150](User%20Guide.assets/image-20220526215441150.png)

### Delete a Fund

To delete the selected fund, press the **\[REMOVE\]** button below the list of funds. You would receive a warning before you can delete the fund:

![image-20220526215603479](User%20Guide.assets/image-20220526215603479.png)

Enter the correct answer to the mathematic question to proceed with the deletion of the fund:

![image-20220526215652333](User%20Guide.assets/image-20220526215652333.png)

The selected fund is now removed from the list of funds and you can no longer access it.