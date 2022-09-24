# time order data visualization 

This is a data visualization project based on Jannchie/Historical-ranking-data-visualization-based-on-d3.js, which easily converts time-order data to dynamic scoll bar chart.  
This project aims to help video creators without programming experience produce time-order animation videos.  
In case, we provide some examples of collecting video infomation and convert the original data to suitable format.   
We also provide codes that can easily help creators convert original data to ranking-data, if you want to use the original codes.  

----
# Changes from Original codes
* Data will be sorted and show by time, rather than value.
* Recording data at every time point is not required anymore. You should provide data in one particular day, and it will be preserved. (It would disappear in the original version)
* Provide a color palette with more colors, as the amount of type has greatly increased.
* Change some showing configs to support long titles.
# How to Use

Open `src/bargraph.html` in any browser and click `choose file` button. Choose your `.csv` formated data source then you can see the visualzied result. 

# Data Format

You can load data source in `.csv` format. See format requirement below:

| name  | type  | value  | date  |
| :---: | :---: | :----: | :---: |
| Name1 | Type1 | Value1 | Date1 |
| Name2 | Type2 | Value2 | Date2 |


**Names** will be displayed as categorical labels on Y-axis. **Name-Type** together will be displayed as annotations on bars.

**Types** are associated with bar colors. Please use type names with no whitespaces or any special characters other than English letters and Chinese characters.

**Values** are associated with bar length. They have to be interger or float values. 

**Dates** should be in `YYYY-MM-DD` format.

# Configurations

You can customize this project by editing parameters in [`src/config.js`](/src/config.js) with any text editor. Please check [`src/config.js`](/dist/config.js) comments for parameter details.

Note that some options may not be available at this point, since I modified the original code a lot.

