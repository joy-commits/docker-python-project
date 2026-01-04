## 📬 Mindfuel Quote Email Service

This is a simple Python service that fetches a daily quote from the ZenQuotes API and sends it via email to recipients stored in a PostgreSQL (Supabase) database. The service is containerized with Docker, making it easy to run anywhere.

### ⚙️ What it does
* Fetches the daily quote from ZenQuotes
* Reads recipient emails from a Supabase PostgreSQL database
* Sends the quote via email
* Runs as a short-lived Docker container

### 🏗️ Architecture Overview
The flow of the service is straightforward:
1.  The container starts and runs the Python application
2.  The app fetches the daily quote from the ZenQuotes API
3.  It connects to the Supabase PostgreSQL database to get email addresses
4.  The quote is sent to the recipients via email
5.  The container exits after completion

### 🐳 Docker Image
The service is available as a Docker image:
```
mindfuel-quote-service
```

### ⬇️ Pulling the Image
```
docker pull mindfuel-quote-service
```

### ▶️ Running the Container
Run the container using your ```.env``` file:
```
docker run --rm --env-file .env mindfuel-quote-service
```
Once started, the container:
* Fetches the daily quote
* Sends the emails
* Exits cleanly

### 🖥️ Output
When run successfully, logs are printed to the terminal showing the progress of the service.
