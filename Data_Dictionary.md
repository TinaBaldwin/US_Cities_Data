# Data Dictionary for US Cinities Connectivity

## combined_data Columns and Descriptions

| Column Name           | Data Type     |   Description |
|-----------------------|---------------|---------------|
| City                  | String        | Name of City  |
| State                 | String        | U.S. state where the city is located |
| Population            | Integer       | Total population of the specific city |
| Avg Income            | int64         | Average Income in the specific city |
| CostOfLiving          | int64         | Cost of living in the specific city |
| Latitude              | float64       | Latitude of the specific city |
| Longitude             | float64       | Longitude of the specific city |
| Walk Score            | float64       | Score reflecting easy it is to walk around a city to complete errands without a car |
| Park Acres            | float64       | Number of acres of public parks in the city |
| Tennis Courts         | int64         | Number of public tennis courts in the city |
| Swimming Pools        | int64         | Number of public swimming pools in the city |
| Tracks                | int64         | Number of public walking/running tracks in the city    |
| Pickleball Courts     | int64         | Number of public pickleball courts in the city |
| Miles of Trails       | int64         | Total miles of trails accessible to public |
| Restrooms             | int64         | Number of public restrooms in the city |
| Basketball Hoops      | int64         | Number of public basketball hoops in the city |
| Community Gardens     | int64         | Number of public community gardens in the city |
| Community Centers     | int64         | Number of public community centers in the city |
| Amenity Cost          | float64       | Ratio of number of amenities to cost of living in the city |
| Amenities by Pop      | float64       | Ratio of number of amenities to population of the city |

## Function Descriptions

| Function Name         | Description  | Parameters  | Return Type |
|-----------------------|--------------|-------------|-------------|
| convert_columns_to_int | Iterates over columns list to convert specific colums in the  dataset to integers | 'df' (data frame), 'columns' (list of items to be converted) | integer |
| convert_columns_to_string | Iterates over the columns list to convert specific columns in the dataset to strings | 'df' (data frame), 'columns' (list of items to be converted) | string |
| extract_null_rows | Iterates over dataframe to locate all the null values | 'df' (data frame) | rows with Nan values |
| fill_null_values | Fills null values with a specified piece of information | 'df' (data frame), 'columns' (list of the columns to have null values replaced), 'fill_value' (value used to replace the null)

## Notes
- Missing value for Park Acres for Des Moines, IA, was filled in using park acres value listed on the city's Parks and Recreation website, https://www.dsm.city/departments/parks_and_recreation-division/, as accessed on 3/11/25. 
- Missing values in "Cost of Living" were filled using state averages.
- The Connectivity dataframe comes from https://www.kaggle.com/datasets/vellis1/us-cities-urban-connectivity/data.
- The us_cities dataframe somes from https://www.kaggle.com/datasets/louise2001/us-cities.

