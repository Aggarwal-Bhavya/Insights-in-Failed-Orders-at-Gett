# Failed Orders Analysis at Gett

## Description

This project explores insights from failed orders in the Gett app. Using Python for data preparation and Tableau for visualization, the project aims to analyze the reasons why some orders did not result in a completed ride.

## Scenario

Gett, formerly known as GetTaxi, is an Israeli-developed technology platform for corporate Ground Transportation Management (GTM). The platform includes an app where customers can request taxis, and drivers can accept these requests. When a customer clicks the Order button, the system searches for available drivers and offers them the order. This analysis focuses on orders that did not proceed as planned, specifically where the customer ended up not getting a car.

## Data Description

The dataset `data_orders` is stored in CSV format and includes the following columns:

- **order datetime**: The time the order was placed.
- **origin longitude**: The longitude of the order's origin.
- **origin latitude**: The latitude of the order's origin.
- **order gk**: The unique identifier for the order.
- **m order eta**: The estimated time before order arrival.
- **order status key**: The status of the order, where:
  - `4` indicates cancellation by the client.
  - `9` indicates cancellation by the system (e.g., rejection).
- **is_driver assigned key**: Whether or not a driver was assigned to the order.
- **cancellation time in seconds**: The number of seconds elapsed before the order was cancelled.

## Preprocessing Code

The data preprocessing is done using Python. You can review the code used for data preparation here:

[Preprocessing Code](https://github.com/Aggarwal-Bhavya/Insights-in-Failed-Orders-at-Gett/blob/main/Failed_Orders_at_Gett.ipynb)

## Results

The visualizations of the failed orders are created in Tableau. You can view the interactive dashboard here:

[Tableau Visualization](https://public.tableau.com/shared/SH4GPJB6P?:display_count=n&:origin=viz_share_link)

Based on visualization results, following recommendations are made:

- Hiring of more drivers as the cancellations are highest when driver waiting time is too long.
- Add more tips for drivers operating at night hours, as they have the minimum cancellations.
- Make drivers spread evenly throught the area.

## Acknowledgements

- Inspired by stratascratch.com
