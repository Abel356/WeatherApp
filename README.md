# WeatherApp
This JavaScript project is a weather application that fetches and displays current weather information for a specified city using the OpenWeatherMap API. The app provides a user-friendly interface where users can input a city name and receive real-time weather details. Below is a detailed description of the functionality and components of the project:

1. **Initialization of DOM Elements**
**Result Element**: result is an HTML element where the weather information will be displayed.
**Search Button**: searchBtn is a button that triggers the weather fetch operation.
**City Input Field**: cityRef is an input field where users enter the name of the city they want to get weather information for.
2. **Fetching Weather Data**
**Get Weather Function**: The getWeather function is the core function that retrieves weather data from the OpenWeatherMap API and updates the UI with the fetched information.
3. **Handling User Input**
**Empty Input Check**: The function first checks if the city input field is empty. If it is, it displays a message asking the user to enter a city name.
**Valid Input Handling**: If the input field is not empty, the function constructs the API URL using the city name and a predefined API key. It then clears the input field to prepare for the next input.
4. **Fetching Data from the API**
**Fetch API Call**: The function makes a fetch request to the OpenWeatherMap API using the constructed URL.
**Handling the Response:**
If the city name is valid and the data is successfully fetched, the function extracts the necessary weather details such as city name, weather condition, description, icon, current temperature, minimum temperature, and maximum temperature.
It then dynamically updates the result element to display these details, including an icon representing the current weather condition.
5. **Error Handling**
**Invalid City Name**: If the city name is not valid or the fetch request fails, the function catches the error and updates the result element to display a "City not found" message.
6. **Event Listeners**
**Search Button Click**: An event listener is added to the searchBtn to trigger the getWeather function when the button is clicked.
**Page Load**: An event listener is added to the window object to call the getWeather function when the page loads, potentially showing default weather information or prompting the user for a city name.
This weather app provides a simple yet effective way for users to get real-time weather updates for any city, enhancing user experience with clear, dynamically updated weather information.
