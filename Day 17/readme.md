# Vehicle Fuel Analytics Dashboard

## Overview

This project generates a fully self-contained HTML dashboard from a vehicle fuel dataset (CSV).

The dashboard analyzes fuel efficiency, operating costs, emissions, maintenance expenses, refueling/recharging behavior, vehicle age impact, and E85 economics.

The output is a single HTML file with:

- No external dependencies
- No CDN usage
- Pure SVG charts
- Embedded CSS and JavaScript
- Responsive design (375px–1440px)
- Dark glassmorphism UI

---

# Required Input

Provide a CSV containing at least the following columns:

| Column Name | Description |
|------------|-------------|
| Fuel_Type | Petrol, Diesel, CNG, E85, EV |
| Fuel_Cost_INR | Fuel cost in INR |
| Distance_km | Distance traveled in kilometers |
| CO2_emitted_kg | CO₂ emissions in kilograms |
| Maintenance_Cost_INR | Maintenance expense in INR |
| Refuel_Recharge_time_min | Refueling/Recharging time in minutes |
| Vehicle_Age_Years | Vehicle age in years |
| Fuel_Price_INR | Fuel price per unit |
| Mileage_kmpl | Mileage or efficiency |

---

# User Inputs

```text
Vehicle : Vehicle Model Name
Fuel    : Petrol / Diesel / CNG / E85 / EV
Usage   : City / Highway / Mixed / Fleet
KM/month: Monthly distance
Car Age : Vehicle age in years
