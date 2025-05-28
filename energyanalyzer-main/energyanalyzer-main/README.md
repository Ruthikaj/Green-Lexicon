# Sustainable Energy Consumption Analyzer

# Built for [GreenLexicon](https://github.com/GunaPalanivel/GreenLexicon.git)

## Overview

The Sustainable Energy Consumption Analyzer is a Streamlit-based web application that helps users evaluate the sustainability of their energy consumption. By inputting their monthly household energy usage and the number of people in their household, the application calculates the per capita energy consumption and provides a sustainability score. The score is accompanied by a personalized recommendation to improve or maintain the user's energy efficiency.

## Features

1. **Energy Consumption Input**: Users can enter their total monthly household energy consumption (e.g., kWh) and the number of people in their household.
2. **Sustainability Score Calculation**: The application calculates a sustainability score based on the user's per capita energy consumption, using a linear interpolation between defined minimum and maximum bounds.
3. **Graphical Representation**: The application displays a bell curve plot to visualize the user's energy consumption in relation to the ideal range, as well as a gauge meter to show the sustainability score.
4. **Personalized Recommendations**: Based on the user's sustainability score, the application provides personalized recommendations to either reduce energy consumption or maintain sustainable habits.

## Usage

1. **Set up the Development Environment**:
   - You can use the provided development container configuration to set up the development environment with the necessary dependencies.
   - Alternatively, you can create a virtual environment and install the required packages manually.

2. **Run the Application**:
   - Start the Streamlit server by running the following command in your terminal:
     ```
     streamlit run Hello.py
     ```
   - The application will open in your default web browser.

3. **Analyze Energy Consumption**:
   - In the application, enter your total monthly household energy consumption and the number of people in your household.
   - The application will display your sustainability score, a visualization of your energy consumption in relation to the ideal range, and personalized recommendations.

## Dependencies

The application relies on the following Python libraries:

- `streamlit`: For building the web application.
- `numpy`: For numerical operations.
- `plotly.graph_objects`: For creating the visualization plots.
- `scipy.stats`: For generating the bell curve distribution.

These dependencies are listed in the `requirements.txt` file, which can be used to install the necessary packages.

## Customization

You can customize the application by modifying the following elements:

1. **Sustainability Score Calculation**: The `calculate_sustainability_score()` function can be updated to use a different formula or adjust the minimum and maximum bounds for energy consumption.
2. **Visualization**: The `plot_bell_curve()` function can be modified to customize the appearance and layout of the bell curve plot.
3. **Recommendation Logic**: The conditional statements in the "Personalized Recommendations" section can be updated to provide more tailored suggestions based on the user's sustainability score.
4. **User Interface**: You can further customize the Streamlit-based user interface, such as the page title, layout, and styling, to match your branding and preferences.

## License

This project is licensed under the [Apache License, Version 2.0](LICENSE).
