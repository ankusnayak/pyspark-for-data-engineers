## Build & Start the Cluster:

Inside the project folder (where docker-compose.yaml file exists), run: ->

```shell
    docker-compose down && docker-compose up -d --build
```

This will:

> Build the custom Jupyter + Spark image
> Start Spark Master, Spark Worker, and Jupyter Notebook

## Submit a Spark Job
To run job.py inside the cluster, execute in vs code terminal:

```shell
    docker exec -it spark-master /opt/spark/bin/spark-submit /opt/spark-app/job.py
```

#### Note: copy that `spark_setup` while creating a new spark folder like new project or new tutorials etc.