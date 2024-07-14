# Assessment Instructions

## Question 1

Write a Python function to calculate the trade performance of a given set of trades executed by a financial firm. The function should take a pandas DataFrame as input with the following columns:

#### Date (datetime64[ns]): The date and time of the trade

#### Symbol (string): The ticker symbol of the traded security

#### Side (string): Either 'buy' or 'sell'

#### Size (float, optional): The number of shares traded (default to 1 if not provided)

#### Price (float): The price at which the trade was executed

Your task is to:

### Choose 10 financial metrics that you believe are the most important for tracking trade performance of a strategy.

### Write a function that takes in this DataFrame and computes these 10 metrics.

### Account for both long and short strategies in your calculations.

### Explain how you compute returns in the case of long-short strategies.

### You have access to an auxiliary function:

def getTickerPrice(ticker: str, date: datetime64[ns]) -> float: # This function returns the price of the security 'ticker' at the given 'date' # For the purpose of this exercise, assume it returns a random number
return random.uniform(1, 100) # Example implementation
Use this function to get the current market price of securities when needed for your calculations.

Your function should:

### Handle potential edge cases (e.g., empty DataFrame, missing values)

### Be efficient in its calculations

### Return a dictionary or pandas Series with the computed metrics

### Please provide the implementation of your function along with comments explaining your choice of metrics and any important calculation details.

## Question 2: Analyzing Nancy Pelosi's Trading Performance

Using the trade performance calculation function you developed in the previous question, we'll now analyze a real-world dataset of trades reportedly made by Nancy Pelosi.

Your task is to:

### Load the attached testData.csv file, which contains Nancy Pelosi's trades, into a pandas DataFrame.

### Ensure the DataFrame matches the format required by your function:

#### Date (datetime64[ns])

#### Symbol (string)

#### Side ('buy' or 'sell')

#### Size (float)

#### Price (float)

Preprocess the data if necessary to match this format.
Apply your trade performance calculation function to this DataFrame.
Interpret the results, focusing on the 10 metrics you chose in your function.
