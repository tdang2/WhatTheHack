# Challenge 05 – Weather Data

## Summary

In this challenge, you are asked to ingest weather data so that taxi trips can be enriched with weather conditions at the time of the trip.

You will:

1. Create an Azure Function to connect to a weather data API…
2. And pass it some coordinates and time information…
3. And retrieve weather data at that location and time…
4. Then store the weather data in Azure Cosmos DB…
5. And lastly, enhance your Power BI visualization to show weather conditions for taxi trips

## Technologies

You’ll use the Dark Sky weather API at <https://darksky.net>. You will need to send queries to the API’s REST endpoint and handle the HTTP response payloads, storing the contained weather data in a Cosmos DB instance. Use an Azure Function to do query the API and persist response data.

You will then connect Power BI to Cosmos DB to retrieve the data and combine it with taxi trip data to show weather conditions for each trip.

## Task 1 – Create a Dark Sky account

Navigate to <https://darksky.net>. Create a free account and note your API key and the format for API calls.
IMPORTANT: free accounts are limited to 1,000 API calls per day. The following tasks are written with this limit in mind.

## Task 2 – Prepare weather API request input data

In this task, prepare a list of no more than 1,000 weather request data points.

You should review the DarkSky APIs, select the API that can give weather conditions for a given location and date/time, understand its required inputs, and then emit suitable data points from the taxi trip data you have been working with.

Each of these data points will be a separate request to the API. Limit to max 1,000 data points, since that is the free DarkSky API call limit per day.

Consider how and where you will store these 1,000 (or less) API request input data records for use by following tasks.

## Task 3 – Prepare Cosmos DB repository

Prepare a Cosmos DB repository to which you will write weather data in task 4.

## Task 4 – Create an Azure Function App to query the DarkSky API and store weather data

In this task, create an Azure Function App that reads in the request input data you prepared in task 2.

For each input data record, your Azure Function should:

1. query the DarkSky API appropriately
2. extract the weather data from the response
3. store the weather data in Cosmos DB

In addition to weather data, don’t forget to think about what you need to store in Cosmos DB to enable you to later combine the right weather data with each taxi trip!

This task is complete when you have the same number of new records in the Cosmos DB repository you created as in the input data you prepared in task 2.

## Task 5 – connect to the weather data in Cosmos DB from Power BI and create an enriched visualization

In the Power BI report(s) you created in Challenge04, connect to your Cosmos DB data.

Create a visualization that shows the taxi trip data you emitted in task 2, enhanced with the correct weather conditions for each trip!
