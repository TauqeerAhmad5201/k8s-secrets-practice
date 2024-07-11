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
