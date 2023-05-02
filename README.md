# PySpark 

This is a repository containing a Dockerfile and scripts to build a Docker image with Jupyter Notebook and PySpark installed. This image can be used as a development environment for working with PySpark.

**Prerequisites**   <br>
Before using this repository, you should have the following installed on your system:
- Docker

**Getting Started**
To use this Docker image, follow these steps:

1. Clone this repository to your local machine:

```bash
git clone https://github.com/EricGrose7/pyspark_jupyter.git
```

2. Build the Docker image using the following command:
```bash
docker build -t pyspark_jupyter .
```
3. Run the Docker container with the following command:
```ruby
docker run -it -p 8888:8888 -v <your_notebook_dir>:/notebooks pyspark_jupyter
```

Replace <your_notebook_dir> with the path to the directory on your local machine where you want to store your Jupyter notebooks. This directory will be mounted inside the Docker container as /notebooks.

Open your web browser and go to http://localhost:8888. This will open the Jupyter Notebook interface.

You can now create new notebooks and start working with PySpark.

**License**
This project is licensed under the MIT License - see the LICENSE file for details.
