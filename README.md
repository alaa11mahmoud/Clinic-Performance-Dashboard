# 🌿 Wellness Clinic Analytics Dashboard (Power BI)

An end-to-end analytics solution for a wellness & coaching practice: from **data collection** (a custom mobile app) to **business insights** (an interactive Power BI dashboard).

## Business Problem
The doctor needed to answer questions that a simple sales report can't:
- How much of her available time is actually being booked?
- Which courses attract real demand, and which are underperforming?
- Are clients coming back, and who are the most engaged ones?
- Is revenue driven by private sessions or public sessions?

## Architecture
**FlutterFlow app** → **Supabase (PostgreSQL)** → **Power BI**

I built the app that generates the data myself, so the dashboard is designed around real operational needs.

## Dashboard Pages & Key Metrics

### 1. Profit
- Total revenue, with a split between **private vs public sessions** (≈91% / 9%)
- **Daily profit trend** by session type
- **Custom tooltip page** (drill-through on hover) showing the exact sessions, clients, and prices behind any data point

### 2. Time: Doctor Occupancy % ⭐
- **Occupancy rate** = booked hours ÷ available working hours
- Daily occupancy trend with a month slicer, to spot under-utilized days
- Gauge showing overall utilization (15.69%), which reveals a lot of unused capacity

### 3. Courses: Absorption Rate ⭐
- **Course absorption rate** = enrolled participants ÷ course capacity
- Ranking of courses by demand vs. revenue per course
- Helps separate "popular" courses from "profitable" ones

### 4. Customers: Engagement & Retention ⭐
- **New clients by month** (acquisition trend)
- **Active customers %** and **Repeat users %** (retention)
- **Top 5 most active clients**
- Client distribution by city

## What makes this project different
- Goes beyond revenue: measures **capacity utilization, demand, and retention**
- Built on **self-collected, structured data** instead of a ready-made Kaggle dataset
- Uses **DAX