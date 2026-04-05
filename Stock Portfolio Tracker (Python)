# Hardcoded stock prices
stock_prices = {
    "AAPL": 180,
    "TSLA": 250,
    "GOOGL": 140,
    "AMZN": 130,
    "MSFT": 300
}

portfolio = {}
total_value = 0

n = int(input("How many stocks do you want to enter? "))

for i in range(n):
    stock = input("Enter stock name: ").upper()
    quantity = int(input("Enter quantity: "))
    portfolio[stock] = quantity

for stock, quantity in portfolio.items():
    if stock in stock_prices:
        value = stock_prices[stock] * quantity
        total_value += value
        print(stock, "value:", value)
    else:
        print(stock, "price not available")

print("\nTotal Investment Value:", total_value)

# Save result to file
with open("portfolio_value.txt", "w") as file:
    file.write("Total Investment Value: " + str(total_value))

print("Result saved in portfolio_value.txt")
