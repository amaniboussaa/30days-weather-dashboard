# Weather Dashboard

This Weather Dashboard application fetches real-time weather data from the OpenWeather API and securely stores it in an AWS S3 bucket. It is designed to demonstrate API integration, cloud storage, and best practices for building scalable applications.

## Features

- **Fetch Weather Data**: Retrieves temperature, humidity, and weather conditions for specified locations.
- **Store Data in S3**: Saves the fetched data in JSON format in an AWS S3 bucket.
- **Error Handling**: Gracefully handles API and AWS-related errors to ensure application stability.
- **Secure Configuration**: Manages sensitive data (like API keys) using environment variables.

## Technologies Used

- **Python**: Core programming language for the application.
- **OpenWeather API**: Provides real-time weather data.
- **AWS S3**: Cloud storage for saving fetched weather data.
- **boto3**: AWS SDK for Python to interact with AWS services.
- **python-dotenv**: Handles environment variables securely.
- **requests**: Simplifies HTTP requests for API calls.

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/GilbertDaniel/-30days-weather-dashboard.git
   cd -30days-weather-dashboard
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure AWS**:

 ```bash
aws configure
```
- Put the Access Key ID and press enter
- Put the secret access key also and press enter
- Leave others as default by pressing Enter

4. **Set Up Environment Variables**:
   - Create a `.env` file in the project directory.
   - Add the following variables:
     ```env
     OPENWEATHER_API_KEY=your_openweather_api_key
     S3_BUCKET_NAME=your_s3_bucket_name
     ```

5. **Run the Application**:
   ```bash
   python src/weather_dashboard.py
   ```

## Key Takeaways

- **Environment Configuration**: Secure sensitive data with `.env` files.
- **Dependency Management**: Use `requirements.txt` for consistent installations.
- **Cloud Integration**: Leverage AWS S3 for scalable storage with proper IAM roles.
- **API Integration**: Simplify API calls with the `requests` library.
- **Error Handling**: Ensure the app is stable and user-friendly.

## Future Enhancements

- Add a front-end interface to display weather data.
- Implement a scheduling feature to fetch weather data periodically.


Feel free to contribute or open issues to improve the application!
