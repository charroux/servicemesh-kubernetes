# servicemesh-kubernetes


## Deploy 
```
kubectl apply -f backend.yml      
kubectl apply -f frontend.yml      
kubectl get pods
```

## Get the gateway address
```
kubectl -n istio-system port-forward deployment/istio-ingressgateway 31380:8080
```

## Check

```
http://localhost:31380/backend/hello
```

```
http://localhost:31380/frontend
```

## Access to the back in the frontend code

### Address of the service registered in the DNS 

https://github.com/charroux/servicemesh-kubernetes/blob/main/FrontEnd/src/main/resources/application.yml


https://github.com/charroux/servicemesh-kubernetes/blob/main/FrontEnd/src/main/java/com/example/FrontEnd/MyWebService.java
