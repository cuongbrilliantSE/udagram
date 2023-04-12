# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
  ![Dockerhub](dockerhub.png)
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
* Travis CI showing a successful build and deploy job
* I use circle ci instead of travis ci for charge fee reason
  ![Pipeline](c.png)
  ![CircleCIpipe](circleCIpipe.png)
  [CircleCI pipeline](https://app.circleci.com/pipelines/github/cuongbrilliantSE/udagram/24/workflows/b3d57ed1-6807-40b6-aa93-660d08b617b4/jobs/30 "Click to view the pipeline")


## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
  ![pods](pods.png)
* To verify Kubernetes services are properly set up

```bash
kubectl describe services
```
 ![services](Screenshot from 2023-04-13 01-57-45.png)
 ![services](Screenshot from 2023-04-13 01-58-51.png)
 ![services](Screenshot from 2023-04-13 02-00-13.png)
 ![services](Screenshot from 2023-04-13 02-00-45.png)
 ![services](Screenshot from 2023-04-13 02-01-19.png)
 ![services](Screenshot from 2023-04-13 02-02-29.png)
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![hpas](Screenshot from 2023-04-13 02-04-03.png)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![logs](Screenshot from 2023-04-13 02-05-29.png)

