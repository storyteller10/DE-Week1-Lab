# Week 1 Data Engineering Lab

## Scenario
A small online shop sends daily order data as a CSV file. A manager wants a reliable summary of valid orders by city.

## Pipeline plan
- Source: `orders.csv` (daily batch file)
- Raw destination: BigQuery table `de_intro.raw_orders`
- Curated output: query results after checking and filtering the data
- User of the output: shop manager

## Local data check
Before reporting, record at least two issues you found in the CSV and what you recommend doing with each.

1. Issue and recommendation: missing value --> verify the city name using the system
2. Issue and recommendation: duplicate --> keep one value

## What the pipeline does
Complete after the lab: In one sentence, describe how the data moves from the source to a useful output.

Raw table: de_intro.raw_orders
- Rows loaded: 8
- Rows with a missing city: 1
- Rows with a non-positive quantity: 1
- Rows returned by the filtered query: 5