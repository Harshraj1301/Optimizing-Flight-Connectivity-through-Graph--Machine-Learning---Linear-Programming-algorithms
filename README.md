# Analyzing and Optimizing Airplane Connectivity

This project focuses on analyzing and optimizing airplane connectivity through Graph, Machine Learning, and Linear Programming algorithms to improve operational efficiency, customer satisfaction, and economic performance.


## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement and Objectives](#problem-statement-and-objectives)
- [Importance of the Study](#importance-of-the-study)
- [Dataset](#dataset)
- [Key Analyses](#key-analyses)
  - [Predicting Flight Arrival Delays](#predicting-flight-arrival-delays)
  - [Airport Profiling (Clustering Analysis)](#airport-profiling-clustering-analysis)
  - [Shortest Path between Two Airports](#shortest-path-between-two-airports)
  - [Optimize Airport Connectivity within a State](#optimize-airport-connectivity-within-a-state)
  - [Optimization of Flight Schedules to Minimize Delay Penalties](#optimization-of-flight-schedules-to-minimize-delay-penalties)

## Project Overview

In this project, we leverage a detailed dataset of nationwide flight operations to tackle key challenges in the aviation industry, aiming to enhance operational efficiency, customer satisfaction, and economic performance.

## Problem Statement and Objectives

The aviation industry faces numerous challenges that directly affect operational efficiency, customer satisfaction, and economic performance. This project aims to address five key problems:

1. **Predict Delays:** Develop predictive models for flight delays to improve passenger satisfaction and optimize airline operations.
2. **Cluster Airports and Identify Hotspots:** Identify and profile hotspot airports to understand regional dynamics and propose targeted improvements.
3. **Find the Shortest Route in Terms of Flying Time:** Enhance route planning to save fuel, reduce carbon emissions, and better allocate resources.
4. **Optimize Routes Within a State:** Improve intra-state connectivity to boost local economies by enhancing access to markets.
5. **Optimize Schedule by Minimizing Total Delay Penalty:** Develop strategies to minimize total delay across the network and maximize flights.

## Importance of the Study

1. **Economic Efficiency:** Reducing delays and optimizing routes can lower operational costs significantly.
2. **Environmental Impact:** Optimizing flight paths and reducing delays can lessen the aviation industry's environmental footprint.
3. **Passenger Experience:** Enhancing predictability and efficiency can increase customer satisfaction and loyalty.
4. **Strategic Planning:** Inform long-term infrastructure and policy decisions for airport authorities and government agencies.

## Dataset

### Flight Data Attributes Description
The dataset provides a comprehensive overview of flight information, including operational details, timings, and delays. Key attributes include:

- **Date and Identification:** FL_DATE, OP_CARRIER_AIRLINE_ID, TAIL_NUM, OP_CARRIER_FL_NUM
- **Airport and Location Codes:** ORIGIN_AIRPORT_ID, ORIGIN, DEST_AIRPORT_ID, DEST
- **Timing and Delays:** CRS_DEP_TIME, DEP_TIME, DEP_DELAY, ARR_TIME, ARR_DELAY, CANCELLED
- **Performance Metrics:** CRS_ELAPSED_TIME, ACTUAL_ELAPSED_TIME, CARRIER_DELAY, WEATHER_DELAY, NAS_DELAY, SECURITY_DELAY, LATE_AIRCRAFT_DELAY

## Key Analyses

### Predicting Flight Arrival Delays
- **Objective:** Develop a predictive model for flight delays to improve scheduling reliability.
- **Methods:** Used Gradient Boosting Classifier with feature engineering and SMOTE for class imbalance.
- **Outcome:** Achieved an accuracy of 71.01% and an ROC AUC of 76.85%.

### Airport Profiling (Clustering Analysis)
- **Objective:** Identify patterns in airport operations related to delays and cancellations.
- **Methods:** Used K-means clustering to group airports based on delay and cancellation characteristics.
- **Outcome:** Identified four clusters with unique delay and cancellation patterns.

### Shortest Path between Two Airports
- **Objective:** Determine the shortest flying time between any two airports.
- **Methods:** Implemented Dijkstra’s Algorithm using NetworkX.
- **Outcome:** Provided actionable insights into the fastest routes based on historical data.

### Optimize Airport Connectivity within a State
- **Objective:** Enhance intra-state connectivity by finding the most efficient routes.
- **Methods:** Used Kruskal’s algorithm to compute the Minimum Spanning Tree (MST) of the airport network.
- **Outcome:** Achieved a significant reduction in total delay by over 93%.

### Optimization of Flight Schedules to Minimize Delay Penalties
- **Objective:** Optimize flight schedules to reduce delay penalties and maximize flights.
- **Methods:** Used linear programming with penalty cost minimization.
- **Outcome:** Reduced total penalty costs by 20.15% with minimal reduction in total flights.
