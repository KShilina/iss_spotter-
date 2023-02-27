# ISS Spotter With Promises and "Callback hell"
 This project is a command line application which provides the user with information about when the International Space Station (ISS) will pass overhead their location. It makes use of three APIs to retrieve the necessary data:
- [ipify](https://www.ipify.org/) is used to fetch the user's IP address.
- [ipwhois](https://ipwhois.io/) is used to fetch the latitude and longitude coordinates of the user's location based on their IP address.
- [iss-flyover](https://iss-flyover.herokuapp.com/json/?lat=YOUR_LAT_INPUT_HERE&lon=YOUR_LON_INPUT_HERE) is used to fetch the next times that the ISS will pass over the user's location based on their latitude and longitude coordinates.
Please note the '''iss-flyover'''API used in this project is actually a third-party API that is built on top of the [Where the ISS at?](https://wheretheiss.at/w/developer)API.

The application is created to run on the command line and is implemented in JavaScript using Node.js. The user is provided with an estimated time and date for the next five times that the ISS will pass over their location.

## Prerequisites
To run this tool, you will need to have [Node.js](https://nodejs.org/en/) installed on your machine.

## How to start
Clone this repository using:

```javascript
git clone git@github.com:KShilina/iss_spotter-.git
cd iss-spotter
```
To install the required dependencies, run the following command in your terminal:
```javascript
npm install
```
## Implementation

## Option 1: Using Callbacks
To use the tool with the callbacks implementation, run the following command in your terminal:
```javascript
node index.js
```
## Option 2: Using Promises
To use the tool with the Promises implementation, run the following command in your terminal:
```javascript
node index2.js
```
This will fetch the user's IP address, latitude and longitude coordinates, and the next times the ISS will pass over their location. The results will be displayed in the terminal.

This tool is implemented using both callbacks and Promises, providing an example of how to work with asynchronous code in Node.js using two different approaches.

Take a look over both solutions as a review. Hopefully the promise based solution is easier compare to implementation with callbacks.