# CPI-calculator
A simple code for easily calculating CPI from SPI and total credits.
# Ask the user how many semesters they have completed
n = int(input("Enter number of semesters: "))

# Variables to keep track of totals
total_credits = 0
weighted_sum = 0

# Repeat once for each semester
for i in range(n):

Ask for SPI and credits of the semester
    spi = float(input(f"Enter SPI of Semester {i+1}: "))
    credits = float(input(f"Enter Credits of Semester {i+1}: "))

Update totals
    total_credits = total_credits + credits
    weighted_sum = weighted_sum + (spi * credits)

# Calculate CPI
cpi = weighted_sum / total_credits

# Display result
print("Your CPI is:", round(cpi, 2))
