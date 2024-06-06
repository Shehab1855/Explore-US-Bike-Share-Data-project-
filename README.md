# Explore US Bike Share Data Project

## Overview
In this project, I used Python to explore data related to bike share systems in three major U.S. cities: Chicago, New York City, and Washington, D.C. The goal was to write code that imports the data, computes descriptive statistics, and creates an interactive terminal experience to present these statistics based on user input.

## Software Used
- Python 3
- NumPy
- Pandas

## Project Steps
1. **Download, Clean, and Preprocess the Data**: Obtain the datasets, clean them, and preprocess them for analysis.
2. **Detect Bike Share Usage Patterns**: Use descriptive statistics to find patterns in the data.
3. **Compare System Usage**: Compare bike share usage between Chicago, New York City, and Washington, D.C. Present the results based on user questions.

## Statistics Computed
### 1. Popular Times of Travel
- **Most common month**
- **Most common day of the week**
- **Most common hour of the day**

### 2. Popular Stations and Trips
- **Most common start station**
- **Most common end station**
- **Most common trip from start to end (i.e., most frequent combination of start and end stations)**

### 3. Trip Duration
- **Total travel time**
- **Average travel time**

### 4. User Info
- **Counts of each user type**
- **Counts of each gender** (only available for NYC and Chicago)
- **Earliest, most recent, most common year of birth** (only available for NYC and Chicago)

## An Interactive Experience
The script creates an interactive terminal experience that answers questions about the dataset based on user input. The interaction is driven by the following questions:

1. **Would you like to see data for Chicago, New York, or Washington?**
2. **Would you like to filter the data by month, day, or not at all?**
3. **(If month) Which month - January, February, March, April, May, or June?**
4. **(If day) Which day - Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, or Sunday?**

The answers to these questions determine the city and timeframe. After filtering the dataset, users will see the statistical results and can choose to start again or exit.

## The Datasets
The project includes three city dataset files:
- **chicago.csv**
- **new_york_city.csv**
- **washington.csv**

Randomly selected data for the first six months of 2017 are provided for all three cities. All three datasets contain the following core six columns:
- **Start Time** (e.g., 2017-01-01 00:07:57)
- **End Time** (e.g., 2017-01-01 00:20:53)
- **Trip Duration** (in seconds - e.g., 776)
- **Start Station** (e.g., Broadway & Barry Ave)
- **End Station** (e.g., Sedgwick St & North Ave)
- **User Type** (Subscriber or Customer)

The Chicago and New York City files also include:
- **Gender**
- **Birth Year**

This project highlights the process of data analysis from data cleaning to presenting insights interactively, demonstrating the practical application of Python, NumPy, and Pandas in real-world scenarios.
