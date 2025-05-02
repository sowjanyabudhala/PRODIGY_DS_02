## Hotel Booking Exploratory Data Analysis (EDA)
## Overview
This project performs an in-depth exploratory data analysis (EDA) on a comprehensive hotel booking dataset containing reservations for both city and resort hotels. The analysis aims to uncover key trends, booking behaviors, and factors influencing cancellations and revenue, providing actionable insights for hotel management.
Note: This project is focused on data analysis and visualization within a Jupyter Notebook and does not include model deployment or application hosting.

## Dataset Description
The dataset consists of over 119,000 rows and 32 columns, each representing a hotel booking record. Key features include:

hotel: Type of hotel (City or Resort)

is_canceled: Whether the booking was canceled (1) or not (0)

lead_time: Days between booking and arrival

arrival_date_year/month/week_number/day_of_month: Booking arrival details

stays_in_weekend_nights / stays_in_week_nights: Nights stayed

adults / children / babies: Number of guests

meal: Meal type selected

country: Customer country of origin

market_segment / distribution_channel: Booking source and purpose

is_repeated_guest: Whether the guest is a repeat visitor

previous_cancellations / previous_bookings_not_canceled: Booking history

reserved_room_type / assigned_room_type: Room types

booking_changes: Number of booking modifications

deposit_type: Deposit policy

agent / company: Booking agent/company ID

days_in_waiting_list: Days on waiting list

customer_type: Customer classification

adr: Average daily rate

required_car_parking_spaces: Parking spaces requested

total_of_special_requests: Number of special requests

reservation_status / reservation_status_date: Final status and date

## Project Workflow
1. Data Loading and Initial Exploration

Load the dataset using pandas.

Inspect data structure, types, and summary statistics.

2. Data Cleaning

Handle missing values in columns like children, country, agent, and company.

Remove duplicate records (over 31,000 duplicates identified).

Convert columns to appropriate data types (e.g., dates, categories, integers).

3. Exploratory Data Analysis

Univariate, bivariate, and multivariate analysis using matplotlib and seaborn.

4. Insights and Conclusions

City hotels are busier and more frequently booked than resort hotels.

About 27% of bookings are canceled; repeat guests are rare (~4%).

Most bookings are for couples or small groups, with short stays.

Online channels and TA/TO are the most common booking sources.

Room assignment mismatches are not a major cause of cancellations.

Revenue (ADR) is higher for certain room types and during peak months.

5. Challenges

High volume of duplicate and missing data.

Data type inconsistencies.

Selection of effective visualization techniques.

## Requirements
Python 3.x
google colab

## Libraries:

numpy

pandas

matplotlib

seaborn

## Install dependencies with:

pip install numpy pandas matplotlib seaborn
Download or clone this repository and ensure the dataset (hotel_bookings.csv) is available.

Open the notebook (hotel_booking-EDA.ipynb) in Jupyter Notebook or Google Colab.

Run the cells sequentially to reproduce the analysis and visualizations.

## File Structure
hotel-booking-EDA/
├── hotel_booking-EDA.ipynb
└── hotel_bookings.csv
## Key Insights
City hotels are preferred over resort hotels (about 61% of bookings).

Most bookings are made online, and TA/TO is the leading distribution channel.

The majority of guests are new; repeat business is low.

Short stays and bookings for two people (couples) are most common.

Room assignment mismatches and longer lead times are not primary causes of cancellations.

Revenue is concentrated in certain months and room types; targeting offers in off-peak months could increase occupancy.


## Acknowledgments
Inspired by open-source hotel booking EDA projects and datasets.

