# US Bikeshare Data Analysis Project

## Overview

This project analyzes bikeshare data from three major US cities: Chicago, New York City, and Washington. The primary goal is to compute various statistics that provide insights into the patterns of bikeshare usage. The program allows users to filter the data by city, month, and day, and then displays statistics such as the most common travel times, popular stations, trip duration, and user demographics.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Functions](#functions)
  - [get_filters](#get_filters)
  - [load_data](#load_data)
  - [time_stats](#time_stats)
  - [station_stats](#station_stats)
  - [trip_duration_stats](#trip_duration_stats)
  - [user_stats](#user_stats)
  - [raw_data_request](#raw_data_request)
  - [main](#main)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project provides a detailed analysis of bikeshare data from three cities in the US. Users can interactively select the city, month, and day to filter the data and view various statistics. The program also offers an option to view raw data.

## Dataset

The dataset includes bikeshare information from three cities:
- Chicago
- New York City
- Washington

Each dataset includes columns such as:
- Start Time
- End Time
- Trip Duration
- Start Station
- End Station
- User Type
- Gender (only available for NYC and Chicago)
- Birth Year (only available for NYC and Chicago)

## Installation

To run this project, you'll need to have Python installed. Additionally, the following Python libraries are required:
- pandas
- numpy

You can install these libraries using pip:

```sh
pip install pandas numpy
```

## Usage

1. Clone the repository to your local machine.
2. Ensure you have the required datasets (`chicago.csv`, `new_york_city.csv`, `washington.csv`) in the same directory as the script.
3. Run the script:

```sh
python bikeshare.py
```

4. Follow the prompts to select the city, month, and day for analysis.

## Functions

### get_filters

Asks the user to specify a city, month, and day to analyze.

**Returns:**
- `city` (str): Name of the city to analyze.
- `month` (str): Name of the month to filter by, or "all" to apply no month filter.
- `day` (str): Name of the day of week to filter by, or "all" to apply no day filter.

### load_data

Loads data for the specified city and filters by month and day if applicable.

**Args:**
- `city` (str): Name of the city to analyze.
- `month` (str): Name of the month to filter by, or "all" to apply no month filter.
- `day` (str): Name of the day of week to filter by, or "all" to apply no day filter.

**Returns:**
- `df` (DataFrame): Pandas DataFrame containing city data filtered by month and day.

### time_stats

Displays statistics on the most frequent times of travel.

**Args:**
- `df` (DataFrame): Pandas DataFrame containing city data filtered by month and day.

### station_stats

Displays statistics on the most popular stations and trip.

**Args:**
- `df` (DataFrame): Pandas DataFrame containing city data filtered by month and day.

### trip_duration_stats

Displays statistics on the total and average trip duration.

**Args:**
- `df` (DataFrame): Pandas DataFrame containing city data filtered by month and day.

### user_stats

Displays statistics on bikeshare users.

**Args:**
- `df` (DataFrame): Pandas DataFrame containing city data filtered by month and day.

### raw_data_request

Prompts the user if they want to see raw data and displays it in chunks of 5 rows at a time.

**Args:**
- `df` (DataFrame): Pandas DataFrame containing city data filtered by month and day.

### main

The main function that ties together all the above functions to create an interactive program.

## Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

This README provides an overview of the project, installation instructions, a description of each function, and guidelines for contributing. By following these instructions, users should be able to understand and use the bikeshare data analysis project effectively.
