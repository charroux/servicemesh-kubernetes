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
