# Get-Amenities (Google API)

## Version 1 (getamenitiesV1.py)
This Python script fetches data from the Google Places API based on specified search parameters and saves the results to an Excel file.

## Description

The script retrieves information about places near a specified location using the Google Places API. It allows customization of search parameters such as radius, keyword, type, and language. The fetched data is then parsed and saved to an Excel file.

## Requirements

- Python 3.x
- pandas
- requests

## Installation

1. Clone this repository to your local machine:

   ```
   git clone <repository-url>
   ```

2. Install the required Python packages:

   ```
   pip install pandas requests
   ```

3. Obtain a Google Places API key from the [Google Cloud Console](https://console.cloud.google.com/apis/credentials) and replace the `API_KEY` variable in the script with your own API key.

## Usage

1. Open the script in a Python environment.

2. Customize the search parameters as needed:
   - `latitude` and `longitude`: The coordinates of the city or location.
   - `radius`: The search radius in meters.
   - `keyword`: A term to be matched against all content that Google has indexed for a place.
   - `type`: Restricts the results to places matching the specified type.
   - `language`: The language code, indicating in which language the results should be returned.

3. Run the script. The fetched data will be saved to an Excel file named `city_amenities.xlsx`.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------


## Version 2 (getamenitiesV2.py)

This Python script fetches data from the Google Places API based on specified search parameters and saves the results to an Excel file. This is an enhanced version of the original script with multithreading capability for improved performance.

## Description

The script retrieves information about places near a specified location using the Google Places API. It allows customization of search parameters such as radius, keyword, type, and language. The fetched data is then parsed and saved to an Excel file. In this version, multithreading with ThreadPoolExecutor is utilized to fetch data for multiple coordinates concurrently, leading to faster execution.

## Requirements

- Python 3.x
- pandas
- requests

## Installation

1. Clone this repository to your local machine:

   ```
   git clone <repository-url>
   ```

2. Install the required Python packages:

   ```
   pip install pandas requests
   ```

3. Obtain a Google Places API key from the [Google Cloud Console](https://console.cloud.google.com/apis/credentials) and replace the `API_KEY` variable in the script with your own API key.

4. Ensure your coordinates are stored in an Excel file with columns for latitude and longitude. Update the `excel_file` variable in the script with the path to your Excel file.

## Usage

1. Open the script in a Python environment.

2. Customize the search parameters as needed:
   - `radius`: The search radius in meters.
   - `keyword`: A term to be matched against all content that Google has indexed for a place.
   - `type`: Restricts the results to places matching the specified type.
   - `language`: The language code, indicating in which language the results should be returned.

3. Run the script. The fetched data will be saved to an Excel file.

## Multithreading

In version 2 of the script, multithreading with ThreadPoolExecutor is used to fetch data for multiple coordinates concurrently, enhancing performance by utilizing parallel processing.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any bugs or feature requests.

## License

