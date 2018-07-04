# Stock-Simulation
Simulate Stock Trading Process Via API Calls on Historical Stock Data 

1. Project Intro

1) The project will take historical stock price data using API and allow users mock the behaviors of stock trading back to Early 2018 with $10000 and see how much money they could make till today.
2) Need to start by searching with a ticker symbol.

2. Design, UI/UX, Site Content
1) Stock Price History, from API
2) There is user input, and only validating when user is searching with empty string or invalid ticker symbol.

3. Dynamic HTML / Interactivity
1) On Search, a stock price chart will be displayed, and will enable users to buy/sell the stock with current price when users click on buy/sell.
2) Users could hover and click to get to trigger functions.

4. API
Alpha Advantage: http://www.alphavantage.co/documentation/
The API is called through ajax and PHP, and the user input “ticker” is the custom parameter that passed in.
The API returns the historical stock prices, and the chart will be displayed based on these prices, and also users will be trading upon changes on prices of different days.

5. Chart
1) Plug-in High Chart: http://www.alphavantage.co/documentation/
The chart will display the price changes of users’ own portfolio and the prices of the single stock.
 
2) Moment.js
Used Moment.js to exclude non-trading days and format the dates to pass into API and High Charts.
 
3) JS Object
JS Object “Portfolio” to save users’ customized portfolio on each day. Object makes it easier to check if a key value is in the object and directly over-write the values.
 
4) Angular JS
Used Angular JS to allow users to immediately get the total prices that they need to pay so that they could compare with the money left for them to buy stocks.
 