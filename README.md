### 🐳 Task 1: Containerizing the Python Service

In Task 1, the Python application was packaged into a Docker image. All dependencies were installed, environment variables were managed using a ```.env``` file, and the application was configured to run automatically inside the container. The image was built, tested locally, and published to a container registry.


### 🔗 Task 2: Multi-Container Setup with Docker Compose

In this task, Docker Compose was used to run the Python application together with a PostgreSQL database. The full stack starts successfully using ```docker compose up --build```, with the app connecting to the database and running without errors.