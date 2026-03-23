# mlops-iris-api
This repository contains a project "Iris Prediction API": A simple API to predict Iris species based on sepal and petal measurements.

## To execute
Run following command on ubuntu machine:

```
make start-project
```

This command will start a project, thereby running docker compose and starting all the conatiners. Then API endpoint can be tested using following command:

```
curl -X POST "http://localhost:8000/predict" \
    -H "Content-Type: application/json" \
    -d '{"petal_length":6.5, "petal_width":0.8}'
```

Run following command to stop the project:

```
make stop-project
```
