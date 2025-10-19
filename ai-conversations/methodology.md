Six-Step Development Overview for get_weather_data(city_name, forecast_period=3)

Step 1 – Requirement 
The project objective was to craft a dependable Python function capable of retrieving real-time weather forecasts for any specified city. The design included an adjustable forecast range parameter. After evaluating options, the wttr.in API was chosen for its simplicity, JSON output, and free usage conditions, aligning well with project limitations.

Step 2 – Preliminary Research
This phase involved exploring the wttr.in JSON API to understand its structure and available endpoints. Simultaneously, the Python requests library was reviewed for effective HTTP communication, focusing on proper request handling, error management, and status verification to ensure resilience against network issues.

Step 3 – Design Blueprint
A pseudocode flow was developed to clarify logical sequencing before implementation:

Build the request URL dynamically based on the input city name.

Fetch data using requests.get().

Convert API responses into Python objects using .json().

Slice forecast data according to the desired number of days.

Guard all network operations with exception handling for robustness.

Step 4 – Implementation
The function was written according to the outlined plan:
