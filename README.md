**Panel Calculator README**
**Overview**
The Panel Calculator is a Python script designed to assist users in determining the optimal layout of solar panels on a specified area from a shapefile. It calculates the number of panels that can be placed, the total area covered, the estimated energy output, and the total cost based on user-defined inputs.

**Features**
Input Shapefile: Accepts a shapefile representing the area where solar panels will be installed.
Panel Specifications: Users can specify the dimensions, cost, and energy output of solar panels.
Area Calculations: Computes usable area after considering buffer zones and eligible area for panel placement.
Output: Generates a new shapefile containing the layout of the placed panels, along with detailed statistics about the installation.

**Requirements**
Python 3.x
Required Libraries:
geopandas
shapely
numpy
Install the required libraries using pip:
"pip install geopandas shapely numpy"

**Usage**
Run the Script: Execute the Python script in your terminal or command prompt. Before usage, please hardcode a desired output path on line 13.

**Provide Inputs:**
Enter the path to the shapefile when prompted.
Input the dimensions (length and width) of one solar panel, or a collection of panels.
Specify the cost per panel / collection.
Output: Upon completion, the script generates:
  A new shapefile containing the panel layout.
  Prints total panels placed, total cost, and estimated energy output in kWh.
  
**Input Parameters**
Shapefile Path: The path to the input shapefile that defines the area of interest.
Panel Length (m): Length of one solar panel.
Panel Width (m): Width of one solar panel.
Cost per Panel: The cost of each solar panel/block of panels (in the specified currency).
Panel Spacing: Space between panels (default is 0.5 meters).
Buffer Zone: Distance from the edge of the reservoir to maintain (default is 0.5 meters).
Coverage Percentage: The percentage of the reservoir to cover with panels (default is 100%).
Energy Output per Panel: Maximum energy output of one solar panel (default is 145 Watt Hours).

**Output Files**
The output shapefile will be saved in the specified output_folder with the naming convention: [input_shapefile_name]_PANELS.shp.
Error Handling
The script includes error handling for invalid file paths, empty geometries, and various other issues that may arise during processing. Relevant error messages will be displayed to guide the user.
Conclusion
The Panel Calculator streamlines the process of planning solar panel installations, providing users with valuable insights into layout, cost, and potential energy generation. Users can visualize and optimize solar panel placement on their specified areas, contributing to sustainable energy solutions.

**License**
This project is licensed under the MIT License. Feel free to modify and use the code for your purposes.

**Acknowledgments**
This README was developed with the assistance of ChatGPT, an AI language model by OpenAI. (https://chatgpt.com/)

