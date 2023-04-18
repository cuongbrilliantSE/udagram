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
  [CircleCI pipeline](https://app.circleci.com/pipelines/github/cuongbrilliantSE/udagram/33/workflows/c1137c87-3ab4-43d0-a0e5-57a8ddb215ee/jobs/39 "Click to view the pipeline")


## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
  ![pods](get_pods.png)
* To verify Kubernetes services are properly set up

```bash
kubectl describe services
```
 ![services](describe_service_1.png)
 ![services](describe_service_2.png)
 ![services](describe_service_3.png)
 ![services](describe_service_4.png)
 ![services](describe_service_5.png)
 ![services](describe_service_7.png)
 ![services](describe_service_8.png)
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![hpas](describe_hpa_1.png)
![hpas](describe_hpa_2.png)
![hpas](describe_hpa_3.png)
![hpas](describe_hpa_4.png)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![logs](log_pods.png)

