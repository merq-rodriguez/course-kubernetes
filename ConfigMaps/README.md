# ConfigMap
```
kubectl get cm
```
Ó
```
kubectl get configmap
```

### Create ConfigMap from literal
```
kubectl create configmap test-cm --from-literal variable1=valor1 
```

### Show an ConfigMap
```
kubectl describe cm test-cm 
```

### Delete an ConfigMap
```
kubectl delete cm test-cm  
```

### Mostrar estructura YAML del ConfigMap a crear:
```
kubectl create configmap test-cm \
  --from-literal variable1=valor1 \
  --from-literal variable2=valor2 \
  --dry-run \
  -o yaml
```

### Open Container

```
➜  kubectl exec -it nginx-cm bash
```
```
$ env
```

# Create ConfigMap from File:
```
kubectl create cm nginx-config-dir --from-file=nginx-config-map
```

