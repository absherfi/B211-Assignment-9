# B211-Assignment-9

Heart Rate and Exercise Data Analysis
Project Overview
This project analyzes the effects of diet and exercise on heart rate, specifically for a gym's partnership with a local elementary school. The goal is to visualize heart rate data and provide an interpretation that can be shared with students to explain how different factors influence heart health. Additionally, this project uses Seaborn’s planets dataset to demonstrate different types of visualizations and extract insights from astronomical data.

Key Objectives
Exercise Data Analysis:
Use heart rate data from Exercise_Data.csv to create:
A heatmap of pulse data.
Categorical plots comparing pulse rates by diet and exercise type.
Summarize conclusions in a format suitable for elementary school students.
Planets Dataset Visualizations:
Use the built-in planets dataset from Seaborn to create:
Two relational plots.
Two distributional plots.
Two categorical plots.
Explain which visualizations best highlight notable insights from the dataset.
Installation
To run this project, you need Python 3.x installed, along with the following libraries:

pandas
numpy
seaborn
matplotlib
sklearn

Class Design and Implementation
This project uses a functional approach rather than Object-Oriented Programming (OOP) since the primary objective is data visualization rather than managing complex data structures or behavior. However, a modular structure could be added if extended features are required.

If we were to convert this into a class-based design, a potential structure could include:

Class: ExerciseDataAnalysis
This class would handle loading, processing, and visualizing heart rate data collected by the gym.

Attributes:
data: Stores the raw DataFrame loaded from Exercise_Data.csv.
pulse_heatmap: Stores the heatmap figure object for pulse data.
pulse_catplot: Stores the categorical plot for pulse rates by diet and exercise type.
Methods:
__init__(self, data_path): Initializes the object, loads the data from a CSV file, and prepares it for analysis.
create_pulse_heatmap(self): Generates a heatmap of pulse data by diet and exercise type.
create_pulse_catplot(self): Creates a categorical plot for pulse rates segmented by diet and type of exercise.
explain_results(self): Summarizes conclusions in simple language for an elementary school audience.

Class: PlanetsDataVisualization
This class would handle loading the planets dataset and creating visualizations.

Attributes:
data: Stores the Seaborn planets DataFrame.
relational_plots: Stores figures for relational plots.
distributional_plots: Stores figures for distributional plots.
categorical_plots: Stores figures for categorical plots.
Methods:
__init__(self): Initializes the object and loads the planets dataset from Seaborn.
create_relational_plots(self): Creates two relational plots using different variables in the dataset.
create_distributional_plots(self): Creates two distributional plots to show the spread of key variables.
create_categorical_plots(self): Generates two categorical plots for examining categorical variables.
describe_insights(self): Provides insights based on the generated visualizations, focusing on notable trends.
Limitations
Lack of Interactivity: The project is limited to static visualizations. For more advanced presentations, interactive plots (using Plotly or similar) could be added.
Data Constraints: Analysis is constrained by the data available in Exercise_Data.csv. Further insights could be obtained with additional health indicators (e.g., blood pressure, age).
Class Structure: While no classes are currently implemented, a class-based structure would improve reusability for complex or larger datasets.
