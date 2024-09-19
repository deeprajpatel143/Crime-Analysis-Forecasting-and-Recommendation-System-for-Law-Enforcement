# Crime Analysis, Forecasting, and Recommendation System for Law Enforcement

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Project Structure](#project-structure)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Dataset](#dataset)
8. [Visualization and Dashboard](#visualization-and-dashboard)

---

## Introduction
The **Crime Analysis, Forecasting, and Recommendation System for Law Enforcement** is a comprehensive tool designed to assist law enforcement agencies in analyzing historical crime data, predicting future crime hotspots, and providing actionable recommendations. The system leverages advanced data science techniques to enable proactive measures for crime prevention and resource allocation.

This project was developed for **Smart India Hackathon (SIH)** 2024.

Project YouTube Link - https://youtu.be/zs_Kzh0o3zQ

## Features
- **Crime Data Analysis**: Perform in-depth analysis on crime statistics based on location, time, and type of crime.
- **Crime Forecasting**: Predict future crime trends and hotspots using historical data.
- **Visual Dashboards**: Interactive dashboards with various types of charts, maps, and graphs for visualizing crime patterns.
- **Recommendations**: Provide strategic recommendations to law enforcement based on predictive insights.
- **Geo-Spatial Mapping**: Map-based crime hotspot detection using tools like Folium and GeoPandas.
- **User-Friendly Interface**: A responsive and intuitive UI developed using modern front-end technologies.
- **Interactive Forms**: Allow law enforcement to submit new crime data through forms and update existing records.

## Tech Stack
- **Frontend**: 
  - Dash and Plotly for interactive graphs and visualizations
- **Backend**: 
  - Python (Flask Framework)
  - Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SQLAlchemy, WTForms
  - GeoPandas and Folium for geospatial analysis
- **Database**: 
  - SQLite (can be switched to PostgreSQL or MySQL)
- **Machine Learning**: 
  - Scikit-learn for crime forecasting and hotspot prediction models
- **Deployment**: 
  - Render/Heroku/Gunicorn
  - Docker for containerization

## Project Structure
```bash
Crime-Analysis-System/
│
├── app/                         # Main Flask app directory
│   ├── __init__.py               # App initialization
│   ├── routes.py                 # API routes
│   ├── models.py                 # Data models and SQLAlchemy configuration
│   ├── utils.py                  # Utility functions for data processing
│   ├── forms.py                  # WTForms for user input
│
├── static/                       # Frontend static files (CSS, JS)
│   └── css/                      # CSS files
│
├── templates/                    # HTML templates
│   └── index.html                # Main dashboard
│
├── notebooks/                    # Jupyter notebooks for data exploration
│
├── Procfile                      # For deployment (Gunicorn)
├── render.yml                    # Render deployment configuration
├── requirements.txt              # Python dependencies
├── README.md                     # This readme file
└── Dockerfile                    # Docker configuration
```

## Installation
Clone the repository:
```bash
git clone https://github.com/your-username/crime-analysis-system.git
Navigate to the project directory:
```
```bash
cd crime-analysis-system
Create a virtual environment and activate it:
```
```bash
python3 -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
Install the required dependencies:
```
```bash
pip install -r requirements.txt
Set up the environment variables:
```
```bash
export FLASK_APP=app
export FLASK_ENV=development
Run the Flask application:
```
```bash
flask run
```
## Usage
Once the application is running, you can access the dashboard in your web browser at http://localhost:5000.

## Main Functionalities:
- Upload crime datasets in CSV/Excel format.
- Analyze historical crime patterns using interactive charts.
- Visualize crime hotspots on the map.
- Generate crime trend forecasts for specific regions.
- Submit new crime reports using forms.


## Dataset
The system supports crime datasets in CSV or Excel format. The dataset should contain the following fields:
- FIR No.
- Date
- Time
- Crime Type
- Station Name
- City
- State

## Visualization and Dashboard
The interactive dashboard includes:
- **Crime Heatmaps:** Visualize the density of crime occurrences in various locations.
- **Bar and Line Charts:** Analyze crime data over time and compare crime types.
- **Prediction Charts:** View future crime trends and hotspots.
