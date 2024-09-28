# BigData & Machine Learning Environment with Docker Compose

This repository contains a complete and configured environment for developing and running Big Data and Machine Learning projects, using Docker Compose to easily manage and create containers. With this setup, you can quickly configure a robust environment for large-scale data processing and machine learning modeling without the need to configure each tool individually.

# Included Tools:

Spark: Fast processing engine for large-scale data, integrated with Hadoop.

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
    docker compose up

    # or background
    
    docker compose up -d
    ```

4. Stop the containers when you're done:

    ```bash
    docker compose down
    ```

Docker Compose will automatically set up all necessary containers and provide access to services via mapped local ports. For example:

Spark UI: http://localhost:8080

# Contributions
Contributions are welcome! Feel free to open a pull request with improvements, new tools, or adjustments.

# License
This project is licensed under the Apache-2.0 license. See the LICENSE file for more details.
