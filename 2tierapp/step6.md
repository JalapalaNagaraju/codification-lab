Run command to create a wordpress deployment
`kubectl apply -f wordpress-deployment.yaml`{{execute}}


Run command to get details about the service, deployment and the pods
`kubectl get svc,deploy,pods`{{execute}}


Run command to access the wordpress site
`minikube service wordpress --url`{{execute}}
