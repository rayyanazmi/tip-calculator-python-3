Sure, here is a README for your tip calculator project:

## Tip Calculator

This is a simple tip calculator program written in Python 3. It takes the total bill amount, the desired tip percentage, and the number of people splitting the bill, and then calculates the amount each person should pay.

### Explanation

The program first prompts the user to enter the total bill amount. The input is converted to a float to handle decimal values. Then, the user is asked to enter the desired tip percentage, choosing from 10, 12, or 15. The input is converted to an integer. Finally, the user is asked to enter the number of people splitting the bill, which is also converted to an integer.

Next, the program calculates the tip amount by multiplying the bill amount by the tip percentage as a decimal. The total bill amount is then calculated by adding the tip amount to the original bill amount. Finally, the bill amount is divided by the number of people to determine the amount each person should pay. The final amount is rounded to two decimal places before displaying it to the user.

### Code Explanation

```python
print("Welcome to the tip calculator.")

bill = float(input("What was the total bill? $"))
tip = int(input("What percentage tip would you like to give? 10, 12, or 15? "))
people = int(input("How many people to spilt the bill? "))
```

This code block prompts the user to enter the bill amount, tip percentage, and number of people splitting the bill. The input is converted to the appropriate data type for further calculations.

```python
tip_as_percent = tip / 100
total_tip_amount = bill * tip_as_percent
total_bill = bill + total_tip_amount
```

These lines calculate the tip amount by converting the tip percentage to a decimal and multiplying it by the bill amount. The total bill amount is then calculated by adding the tip amount to the original bill amount.

```python
bill_per_person = total_bill / people
final_amount = round(bill_per_person, 2)
```

These lines calculate the amount each person should pay by dividing the total bill amount by the number of people. The final amount is rounded to two decimal places for better presentation.

```python
print(f"Each person should pay: ${final_amount}")
```

This line prints the final amount each person should pay, using f-string formatting to include the dollar symbol.

I hope this explanation is helpful.
