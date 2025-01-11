# BigData & Machine Learning Environment with Docker Compose

This repository contains a complete and configured environment for developing and running Big Data and Machine Learning projects, using Docker Compose to easily manage and create containers. With this setup, you can quickly configure a robust environment for large-scale data processing and machine learning modeling without the need to configure each tool individually.

# Included Tools:

Apache Datafusion and Ballista: DataFusion is a high-performance in-memory query engine for SQL and data analytics. Ballista is a distributed compute platform for large-scale data processing built on Apache Arrow and DataFusion.
MinIO: Is a high-performance, open-source object storage system compatible with the S3 API, designed for scalability and cloud-native applications.
MLflow: Is an open-source platform for managing the machine learning lifecycle, including experimentation, reproducibility, deployment, and model registry.
pgAdmin: Is an open-source, web-based management tool for PostgreSQL that provides a user-friendly interface for database administration and querying.
PostgreSQL: Is a powerful, open-source relational database management system known for its extensibility, robustness, and SQL compliance.
Prefect: Is a workflow orchestration tool for building, running, and monitoring data workflows.

# Prerequisites
Docker installed on your system.
Docker Compose configured.

# How to use
1. Clone this repository:

    ```bash
    git clone https://github.com/cemarchi/bigdata-docker-compose-sandbox.git
    ```

2. Navigate to the project folder:

    ```bash
    cd bigdata-docker-compose-sandbox-main
    ```

3. Run Docker Compose:

    ```bash
    docker-compose --env-file config.env up --build

    # or background
    
    docker-compose --env-file config.env up -d --build
    ```

4. Stop the containers when you're done:

    ```bash
    docker-compose down
    ```

Docker Compose will automatically set up all necessary containers and provide access to services via mapped local ports. For example:

MinIO UI: http://localhost:9001/
MLflow UI: http://localhost:5000/
PGAdmin UI: http://localhost:8090/
Prefect UI: http://127.0.0.1:4200

# Contributions
Contributions are welcome! Feel free to open a pull request with improvements, new tools, or adjustments.

# License
This project is licensed under the Apache-2.0 license. See the LICENSE file for more details.
