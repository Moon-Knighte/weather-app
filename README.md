In this simple and plain weather app includes fundamental concepts of js and react library and they are demonstrated pointwise below:

1. React State Management: The app utilizes React's state management capabilities to store the weather data(`weather`), the input city name (`inputCity`), and update them when needed.

2. useState Hook: The `useState` hook is used to declare state variables `weather` and `inputCity` within the functional component 'WeatherApp'.

3. API Data Fetching: The app fetches weather data from the OpenWeatherMap API using the Axios library. It sends an HTTP GET request to the API endpoint with specified city name to retrieve weather information.

4. Asynchronous JavaScript: Asynchronous JavaScript is used to handle the asynchronous nature of data fetching operations. The `fetchWeather` function is declared as `async`, and `await` is used to asynchronously fetch weather data from the API.

5. Conditional Rendering: The app conditionally renders weather infromation based on weather the `weather` state variable is not null. If `weather` contains data, it renders weather information; otherwise, it does not display anything.

6. Event Handling: Event handling is used to capture user input when they type in a city name and when they click the search button. The `onChange` event on the input field updates the `inputCity` state variable, and `onClick` event on the button triggers the `handleSearch` function.

7. Error Handling: Error handling is implemented to catch any errors that may occur during the API request. If an error occurs, it's logged to the console for dibugging purposes.

8. Dynamic API URL: The API URL is dynamically constructed using template literals to include the input city name and API key stored in environment variables.

9. Environment Variables: The API key is stored securely as an environment variable (`REACT_APP_WEATHER_API_KEY`) to prevent exposing it in the codebase. Environment variables are accessed using `process.env` in the js code.

10. Metric Units: The API requests specifies the unit of measurement for temprature as Celsius(`units=metric`), ensuring consistency in displaying temprature data.
