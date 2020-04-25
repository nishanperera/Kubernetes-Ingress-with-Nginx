# Kubernetes Ingress controller with Nginx

## Install Nginx

https://kubernetes.github.io/ingress-nginx/

## Check that it’s all set up correctly

<code>kubectl get pods -n ingress-nginx</code>

## Create first application
<code>kubectl apply -f app1.yaml -f app1-service.yaml</code>

## Create second application
<code>kubectl apply -f app2.yaml -f app2-service.yaml</code>

## Create ingress controller
<code>kubectl apply -f ingress.yaml</code>

## Test applications
<code>curl -kL http://localhost/app1</code>

<code>curl -kL http://localhost/app1</code>

