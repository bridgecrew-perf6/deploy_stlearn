# deploy_stlearn

## Workflow

- Step 1:

```
git clone https://github.com/duypham2108/deploy_stlearn.git
cd deploy_stlearn
git clone https://github.com/BiomedicalMachineLearning/stlearn_interactive.git flask_app
```

- Step 2:

```
bash run_docker.sh
```

- Step 3: Check the container ID of docker by

```
docker ps -a
```

And get the second container.

- Step 4: Check the IP address of the container

```
docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' <The container ID>
```

- Step 5: Access stLearn at `<IP address>:8000`
