
# Go Basic Web Server

A basic Go web server project that exposes an API endpoint for greeting visitors.

[GitHub Repository](https://github.com/joshua468/go-basic-web-server)

## Overview

This project implements a simple Go web server that responds to GET requests on `/api/hello`. It returns a JSON response with the client's IP address, hardcoded location (`New York`), and a greeting message that includes the visitor's name and a temperature value.

## Installation

**Clone the repository**:
```bash
git clone https://github.com/joshua468/go-basic-web-server.git
cd go-basic-web-server

Start the server:
bash
Copy code
go run main.go
This command starts the Go web server on your local machine.

Access the API endpoint:
Open a web browser and navigate to http://localhost:8080/api/hello?visitor_name=Mark (replace Mark with any name).

Usage
Send a GET request to the following endpoint to get a greeting message:

javascript
GET <your-server-url>/api/hello?visitor_name=Mark
Replace <your-server-url> with the actual URL where your server is hosted.

Example Response:
json
Copy code
{
  "client_ip": "127.0.0.1",
  "location": "New York",
  "greeting": "Hello, Mark!, the temperature is 11.0 degrees Celsius in New York"
}
This JSON response format includes the client's IP address, hardcoded location (New York), and a greeting message with the visitor's name and temperature.