# Progressive Web App: Budget-Tracker
Full stack Budget Tracker Progressive Web Application using a Service Worker, IndexedDB, and the Cache API to allow for offline access and functionality, in front of Express and Mongoose.

## Deployed URL: https://budget-tracker-cbraggdev.herokuapp.com/

## Features

The user will be able to add expenses and deposits to their budget with or without a connection. When entering transactions offline, they should populate the total when brought back online.

Offline Functionality:

  * Enter deposits offline

  * Enter expenses offline

When brought back online:

  * Offline entries should be added to tracker.


![Budget-Tracker-Demo](https://media.giphy.com/media/TL6lyL4VtCOMPbYc6z/giphy.gif)

## Instructions for Offline Functionality Test
1) In Google Dev Tools > Application > Service Workers, enable "Offline" setting.  
2) Enter transactions by adding or subtracting funds.
3) Transactions entered while offline are saved in IndexedDB "pending" object store.  
4) Going "Online" will trigger the API calls to the MongoDB to catch up the database transactions.  

## User Story
AS AN avid traveller  
I WANT to be able to track my withdrawals and deposits with or without a data/internet connection  
SO THAT my account balance is accurate when I am traveling  

## Business Context
Giving users a fast and easy way to track their money is important, but allowing them to access that information anytime is even more important. Having offline functionality is paramount to our applications success.