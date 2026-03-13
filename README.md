# CPU Cooler Performance Analysis (MATLAB)

## Overview
This project is a hands-on thermal analysis of CPU cooling performance using BIOS-based fan control, HWiNFO sensor logging, and MATLAB-based visualization. Inspired by my interest in PC building, I tested how different CPU fan settings affect temperature behavior during both load and cooldown conditions.

## Objective
The goal of this project was to evaluate how fan-speed changes influence CPU temperature and cooling efficiency. In particular, I compared peak temperature during stress, cooldown behavior after the load was removed, and overall temperature trends across multiple fan settings.

## Method
- Adjusted CPU fan settings in BIOS under controlled system conditions
- Used fixed fan settings of 20%, 40%, 60%, 80%, and 100% for comparison
- Started each test from a thermally stable idle condition at approximately 2–5% CPU utilization
- Applied CPU stress for 2 minutes, then removed the load and observed cooldown behavior for 1 minute
- Logged CPU temperature and package power using HWiNFO
- Exported the sensor data as CSV files and processed them in MATLAB to generate temperature-response graphs

## Result
Temperature-response graphs were generated to compare CPU thermal behavior under different fan settings. Although the differences were not dramatic, higher fan-speed settings generally reduced peak temperature during stress and improved post-load cooling performance. Lower fan settings, particularly in the 20% to 60% range, tended to retain higher temperatures for longer and cool down more slowly.

## System Setup
- **CPU:** AMD Ryzen 5 5600X
- **Motherboard:** MSI MAG B550M MORTAR WIFI
- **Cooler:** Thermalright Assassin Spirit 120 EVO Black
- **Fan:** 120 mm PWM Quiet ARGB Fan  
- **Maximum Fan Speed:** approximately 2200 RPM

## Tools Used
- BIOS fan control
- HWiNFO
- MATLAB

## Files
- `cpu_cooler_analysis.m` — MATLAB script for importing CSV data and generating graphs
- `fan20.csv` — logged sensor data for 20% fan setting
- `fan40.csv` — logged sensor data for 40% fan setting
- `fan60.csv` — logged sensor data for 60% fan setting
- `fan80.csv` — logged sensor data for 80% fan setting
- `fan100.csv` — logged sensor data for 100% fan setting

## Key Takeaway
This project demonstrates a simple experimental workflow for thermal analysis by combining hardware-level fan control, real-time sensor logging, and MATLAB-based data visualization. It also shows how relatively small airflow changes can still produce measurable differences in cooling behavior under real operating conditions.
