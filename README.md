[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/) 

## Overview
This is Python web application is written using [Flask](https://flask.palletsprojects.com/en/2.0.x/) framework. Application shows for you current date and time in Moscow zone (GMT+3)

## Getting started 
To get the application up and running (locally or in Docker) follow these simple steps. 

### Locally 
Before running the application, please install its prerequisites:
* [Python](https://www.python.org/downloads/)
* [pip](https://pip.pypa.io/en/stable/installation/)

To run from the master branch, follow the instructions below:
1. Clone web application repository locally.
    ```bash
    git clone https://github.com/rufusnufus/devops
    cd devops/app_python/
    ```
2. Create virtual environment.
    ```bash
    python -m virtualenv venv 
    source venv/bin/activate
    ```
3. Install packages.
    ```bash
    pip install -r requirements.txt
    ```
4. Run the application. Web app will open at [http://localhost:5000/](http://localhost:5000/).
    


### Docker installation
Before running the application, please install its prerequisites:
* [Docker 20.10.7+](https://docs.docker.com/get-docker/)

To run from the master branch, follow the instructions below:
1. Clone web application repository locally.
    ```bash
    git clone https://github.com/rufusnufus/devops
    cd devops/app_python/
    ```
2. [Optional] Build the image.
    ```bash
    docker build -t nufusrufus/devops .
   ```
3. Run the container. Web app will open at [http://localhost:8000/](http://localhost:8000/).
    ```
    docker run -p 8000:8000 nufusrufus/devops
    ```

### Unit Testing
1. Make sure that you are in the application directory:
    ```bash
    cd devops/app_python
    ```
2. Run the tests:
    ```bash
    pytest tests
    ```
