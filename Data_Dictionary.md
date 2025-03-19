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
| us_cities_int         | Iterates over the city_column list to convert specific colums in the us_cities dataset to integers | 'us_cities' (data frame), 'city_columns' (list of strings) | integer |
| us_cities_string | Iterates over the city_column list to convert specific columns in the us_cities dataset to strings | 'us_cities' (data frame), 'city_column' (list of strings) | string |
|extract_null_rows_cities | Iterates over us_cities to locate all the null values | us_cities (data frame) | rows with Nan values |
| connectivity_int | Iterates over the columns list to convert specific columsn in the connectivity dataset to integers | 'connectivity' (data frame), 'column' (list of strings) |
| connectivity_string | Iterates over columns list to convert specific columns in the connectivity data frame to strings | 'connectivity' (data frame), 'column' (list of strings) | string |
| extract_null_rows | Iterates over connectivity data frame and returns all rows with null values | 'connectivity' (data frame)  | rows wtih Nan values |
| connectivity_null | Fills in the null value for a specified column wtih a specified value | 'connectivity' (data frame), 'column' (list) | does not return anything, replaces a value |

## Notes
- Missing value for Park Acres for Des Moines, IA, was filled in using park acres value listed on the city's Parks and Recreation website, https://www.dsm.city/departments/parks_and_recreation-division/, as accessed on 3/11/25. 
- Missing values in "Cost of Living" were filled using state averages.
- The Connectivity dataframe comes from https://www.kaggle.com/datasets/vellis1/us-cities-urban-connectivity/data.
- The us_cities dataframe somes from https://www.kaggle.com/datasets/louise2001/us-cities.

