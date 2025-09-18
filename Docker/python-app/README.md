# Python Application

## Overview
This project is a Python application that utilizes Flask as a web framework. It includes essential dependencies such as requests and numpy, and is containerized using Docker for easy deployment.

## Setup Instructions

1. **Clone the Repository**
   Clone this repository to your local machine using:
   ```
   git clone <repository-url>
   ```

2. **Navigate to the Project Directory**
   Change into the project directory:
   ```
   cd python-app
   ```

3. **Build the Docker Image**
   Run the following command in the terminal from the project root directory:
   ```
   docker build -t python-app .
   ```

4. **Run the Docker Container**
   Execute the following command to run the container:
   ```
   docker run -p 5000:5000 python-app
   ```

## Usage
Once the container is running, the application will be accessible at `http://localhost:5000`. You can interact with the application through your web browser or any API client.

## Dependencies
This project requires the following Python packages:
- Flask
- requests
- numpy

These dependencies are listed in the `requirements.txt` file and will be installed automatically when building the Docker image.

## Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request with your changes.