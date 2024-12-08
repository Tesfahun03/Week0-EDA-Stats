                                    README: Visualizing Environmental Data Relationships
Overview
This script visualizes relationships and distributions within an environmental dataset. It leverages Matplotlib and Seaborn to produce insightful plots, including scatter plots, histograms, and bubble charts. These visuals help analyze key variables such as solar radiation, temperature, wind speed, and relative humidity.
Features

    Scatter Plot: Temperature vs. Relative Humidity
        Purpose: Explore the relationship between ambient temperature (Tamb) and relative humidity (RH), with solar radiation (GHI) as a hue.
        Visualization Details:
            X-axis: Relative Humidity (RH) in percentage (%)
            Y-axis: Ambient Temperature (Tamb) in degrees Celsius (°C)
            Hue: Global Horizontal Irradiance (GHI) to show additional context
            Color Palette: viridis

    Histograms: Key Variables
        Purpose: Visualize the frequency distribution of critical variables, including:
            Solar Radiation Components: GHI, DNI, DHI
            Wind Speed (WS)
            Ambient Temperature (Tamb)
        Visualization Details:
            Number of bins: 20
            Color: Teal
            Edge Color: Black
            Layout: Multiple histograms displayed together for comparison

    Bubble Chart: GHI vs. Tamb vs. WS
        Purpose: Examine the interplay between solar radiation, temperature, and wind speed, with bubble size representing relative humidity (RH).
        Visualization Details:
            X-axis: Global Horizontal Irradiance (GHI)
            Y-axis: Ambient Temperature (Tamb)
            Bubble Size: Normalized RH values
            Bubble Color: Wind Speed (WS) represented using the coolwarm colormap
            Transparency (alpha): 0.7 for clear visual distinction
            Edge Color: Black for bubbles

Dependencies

    Python Libraries:
        matplotlib: For plotting charts
        seaborn: For advanced visualizations and scatter plots
        numpy (optional): For any required numerical operations

Install Requirements:

    pip install requirements.txt file to install all dependencies

How to Run

    Ensure you have the required Python libraries installed.
    Replace data in the script with your dataset. The dataset should include the following columns:
        RH: Relative Humidity (%)
        Tamb: Ambient Temperature (°C)
        GHI: Global Horizontal Irradiance
        DNI: Direct Normal Irradiance
        DHI: Diffuse Horizontal Irradiance
        WS: Wind Speed
    Run the script in a Python environment that supports graphical output (e.g., Jupyter Notebook, Python IDE).

Sample Output

    Scatter Plot: Visualizes the relationship between temperature and humidity, highlighting patterns influenced by solar radiation.
    Histograms: Provide insights into the distribution of key variables, helping identify trends or anomalies.
    Bubble Chart: Offers a multi-dimensional view of solar radiation, temperature, and wind speed, with bubble size adding additional context.

Customizations

    Change Hue/Color Mapping:
        Modify the hue parameter in the scatter plot or the colormap in the bubble chart to focus on other variables.

    Adjust Plot Aesthetics:
        Change figsize, alpha, or color palettes to match your preferred style.

    Extend Visualizations:
        Add additional plots or include other variables from the dataset for deeper analysis.

License

Feel free to use and modify this script for personal or educational purposes. Attribution is appreciated.