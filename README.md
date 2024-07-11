### Let's see how we can create secret 

General Syntax: 
```
kubectl create secret <secret type> <secret name> --from-literal=<key>=<value>
```

```
kubectl create secret <secret type> <secret name> --from-file=<key>=<value>
```

Types of Secrets: 

- Generic
- Docker-registry
- TLS

Ref to file- secret-1.yaml (Generic Type)
``` 
kubectl create secret generic db-secret --from-literal=username=dbuser --from-literal=password=23cfged
```

Ref to file- secret-2.yaml (Docker Registry)
```
kubectl create secret docker-registry docker-secret --docker-email=hellotauqeer@gmail.com --docker-username=dev --docker-password=pass1234 --docker-server=my-registry.example:5000
```
