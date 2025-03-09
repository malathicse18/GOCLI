GoCLI - Fetch Logs from MongoDB

Overview

GoCLI is a command-line and API-based tool for fetching logs from MongoDB. It allows users to retrieve logs using both CLI commands and a RESTful API.

Prerequisites

Go (latest version)

MongoDB running on mongodb://localhost:27017

Installation

Clone the repository and initialize the Go module:

git clone <repo-url>
cd gocli
go mod tidy

Usage

Run CLI to Fetch Logs

go run main.go logs --db=myDatabase --collection=myCollection

This will fetch and pretty-print logs from the specified database and collection.

Start API Server

go run main.go api --db=myDatabase --collection=myCollection

The API will be available at:

http://localhost:8080/logs

You can fetch logs via an HTTP GET request.

Features

Fetch logs from MongoDB using CLI.

Start a REST API to retrieve logs.

Pretty-print logs in JSON format.

License

This project is licensed under the MIT License.

Contributing

Feel free to open issues or contribute via pull requests!
