---
title: "WeatherStack"
sidebar:
  exclude: true
---
## Introduction

This project involves the development of a console based weather application that uses the Weatherstack API to fetch and display current or historical weather data. The primary goal is to enable users to input a city location and receive detailed weather information, including UV index, temperature, humidity, wind speed, and more. Designed with accessibility and ease of use in mind, this will offer an efficient and accessible tool for users to check the weather condition for any specified location.

## Objectives

The main objectives for this project are to ensure data accessibility, error management and API integration all within the C programming language and using a Linux machine. Data accessibility includes offering real time weather information based on a location’s identifiable information with an easy to use user interface. Error management involves implementing a robust error handling to manage invalid inputs and unsuccessful API calls. Doing so will enhance the reliability and offer user feedback. Lastly, API integration involves the use of the Weatherstack API along with the libcurl and jsmn libraries to facilitate API communication and JSON parsing.

## Program Architecture

The program code will be made in a modular fashion meaning the code will be created in chunks which will allow it to be more manageable and each code block serving as a building block for the entire program. The blocks are as follows:

- **Input Block:** This block will prompt and collect user input (e.g. city name) and include necessary code for validating the user’s input.
- **API Block:** This block of code will establish the connection with the Weatherstack API by sending an HTTP request and handling the response with the help of the libcurl library.
- **Data Processing:** This block will contain the code for parsing the API response which will be in a JSON format. This code will utilize the jsmn library, or similar, to organize the relevant data into a C data structure.
- **Output/Display Block:** This block will take the data structure and will display the parsed data to the user in a console friendly format.

Additionally, the code will be compiled with the gcc compiler.

## Program Flow

The program will first welcome the user and introduce the weather functionality (e.g. offer an example input). Then the user will provide an input. The program will validate the input and if valid will make an API call to retrieve the weather data for that location. The response to the call will then be parsed and presented to the user. If input is invalid or if the call fails, the program will provide error handling and prompt the user to retry.

## Procedure

1. Create WeatherStack Account
   - Navigate to <https://weatherstack.com/> and create an account. Once the account is made you will be presented with your API key
2. Install libcurl

   ```bash {filename="bash"}
   sudo apt-get install libcurl4-openssl-dev
   ```
