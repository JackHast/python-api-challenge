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
 
In the jupyter notebook WeatherPy.ipynb firstly 1500 coordinates have been randomly generated. Using the module citipy the nearest city for each set of coordinates has been determined and stored in the list 'cities' of which 592 cities have been found. Using the openweather api, weather information such as max temperature, humidity, windspeed, etc., have been fetched and stored in the pandas dataframe city_data and exported as a csv file located in the folder 'data'.

This data has then been used to determine whether there exists any correlation between temperature and latitude, humidity and latitude, cloudiness and latitude, windspeed and latitude via calculating the pearson coefficient and plotting a line of best fit for each data set which has been done for northern and southern hemispheres separately. 
The results indicate that though there is a clear correlation between latitude and max temperature, there is at best a weak correlation between latitude and humidity, windspeed and cloudiness. 

In the notebook VacationPy.ipynb the data generated in WeatherPy.ipynb is mapped by firstly using geoapify to find the coordinates of each city and then hvplots to plot each city. Next, the dataframe city_data_df is filtered for cities with certain attributes such as max temperature between 21-27 degrees and geoapify is again used to find a hotel within the city which is then mapped using hvplots. 



