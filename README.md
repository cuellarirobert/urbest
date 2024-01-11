# README for Flask and JavaScript-Based Work Order Application

## Overview
This application provides an interactive solution for managing work orders, utilizing Flask for the backend and JavaScript for the frontend. It integrates MapsIndoors JavaScript SDK and Mapbox GL JS for mapping functionality, alongside Urbest for issue tracking and management.

## Key Features
- **Interactive Indoor Maps:** Powered by MapsIndoors JavaScript SDK and Mapbox GL JS.
- **Work Order Management:** Submission and tracking of work orders via a user-friendly interface.
- **Dynamic Content:** Categories and building information are dynamically loaded and displayed.
- **Geodata Handling:** Creation and management of geodata points on MapsIndoors maps.
- **Urbest Integration:** Issue drafting and publishing through Urbest's API.

## Frontend
- **HTML & Bootstrap:** Structured and styled user interface.
- **JavaScript:** Controls the application logic, including map interactions and form handling.
- **MapsIndoors Components:** Custom elements for enhanced map functionality.

## Backend (Flask)
- **API Routes:** Handles work order creation, category fetching, and geodata management.
- **Error Management:** Robust error handling for API interactions and internal processes.

## Requirements
- Python 3.x
- Flask
- JavaScript (ES6+)
- MapsIndoors JavaScript SDK
- Mapbox GL JS

## Installation
1. Clone the repository to your local machine.
2. Install Python dependencies: `pip install -r requirements.txt`.
3. Set necessary environment variables (API keys for MapsIndoors, Mapbox, etc.).
4. Launch the Flask app: `python app.py`.

## Configuration
- **Environment Variables:** Required for API keys and other sensitive data.

## Usage
1. Access the web application through the provided URL.
2. Interact with the map to select work order locations.
3. Complete the form to submit a work order.
4. Manage and track the work orders through the Urbest interface.

## Main JavaScript Functions
- `initializeMapClicks`: Handles map click events for work order location selection.
- `createIssue`: Submits issue data to the backend for processing.
- `populateVenueSelector` and `populateBuildingSelector`: Dynamically populate dropdowns based on MapsIndoors data.
- `handleGeoDataResponse`: Manages the response from geodata creation API calls.

## API Endpoints
- `/createGeoData`: Endpoint for creating geodata.
- `/create_issue`: Endpoint for issue creation in Urbest.
- `/get_parent_id`: Retrieves parent ID for a selected map location.

## Contributing
Contributions to enhance features or fix issues are welcome. Please adhere to standard coding practices and submit pull requests for review.

## License
MIT License
