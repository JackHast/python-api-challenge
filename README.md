# Python api Challenge

# Contents of Repository 
The following code contains two folders code and data. code contains two jupyter notebooks VacationPy.ipynb and WeatherPy.ipynb and data contains a csv file cities.csv with data generated in the WeatherPy.ipynb file along with four images. Api keys for both geoapify and openweatherapi are required to run both jupyter notebooks but have been omitted.

Dependencies required to run code files:

- matplotlib.pyploy
- pandas
- numpy requests
- time
- scipy
- citipy
- hvplot

# Summary of Analysis
 
In the jupyter notebook WeatherPy.ipynb firstly 1500 coordinates have been randomly generated. Using the module citipy the nearest city for each set of coordinates has been determined and stored in the list 'cities' of which 592 cities have been found. Using the openweather api, weather information such as max temperature, humidity, windspeed, etc., have been fetched and stored in the dictionary city_data, this dictionary has then been converted to a pandas dataframe and exported as a csv file located in the folder 'date'.
This data has been used to determine whether there is any correlation between temperature and latitude, humidity and latitude, cloudiness and latitude, windspeed and latitude by determining pearson coefficient and 
