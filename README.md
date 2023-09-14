# YouTube Data Migration Project

This project aims to build a data migration pipeline for retrieving and analyzing YouTube channel data using Streamlit, MongoDB, and a SQL data warehouse. The pipeline involves setting up a Streamlit app, connecting to the YouTube API, storing data in a MongoDB data lake, migrating data to a SQL data warehouse, and displaying the data in the Streamlit app.

## Approach

1. Set up of a Streamlit app: Streamlit is an excellent choice for quickly building data visualization and analysis tools. We will create a simple UI where users can enter a YouTube channel ID, view channel details, and select channels to migrate to the data warehouse.

2. YouTube API: We will utilize the YouTube API to retrieve channel and video data. The Google API client library for Python will be used to make requests to the API, allowing us to gather the required data efficiently.

3. Data storage in a MongoDB data lake: Once the data is retrieved from the YouTube API, we will store it in a MongoDB data lake. MongoDB is a suitable option for storing unstructured and semi-structured data, making it a natural fit for our project.

4. Migrate data to a SQL data warehouse: As we collect data for multiple channels, we will migrate it to a SQL data warehouse. MySQL or PostgreSQL, among other SQL databases, can be used for this purpose, providing a structured and query-friendly environment.

5. Query the SQL data warehouse: SQL queries will be employed to join the tables in the SQL data warehouse and retrieve data for specific channels based on user input. Libraries such as SQLAlchemy in Python can be utilized to interact with the SQL database.

6. Display data in the Streamlit app: The final step involves displaying the retrieved data in the Streamlit app. Streamlit's built-in data visualization features will enable us to create charts and graphs, aiding users in analyzing the data effectively.


## Usage

Once the Streamlit app is running, follow these steps:

1. Enter a YouTube channel ID in the provided input field.
2. Click the "Get data and store" button to fetch the channel information.
3. Select the channels you wish to migrate to the data warehouse.
4. Click the "To MySQL" button to initiate the migration process.
5. Use the interactive charts and graphs in the app to explore and analyze the migrated data.
