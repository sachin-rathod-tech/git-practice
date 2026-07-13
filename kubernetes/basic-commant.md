# ☸️ Kubernetes Basic Commands

## Cluster Information

```bash
kubectl cluster-info
```
Shows cluster information.

```bash
kubectl version
```
Displays Kubernetes client and server versions.

```bash
kubectl get nodes
```
Lists all worker nodes.

---

## Namespace

```bash
kubectl get namespaces
```

```bash
kubectl create namespace dev
```

```bash
kubectl delete namespace dev
```

---

## Pods

```bash
kubectl get pods
```

```bash
kubectl get pods -o wide
```

```bash
kubectl describe pod <pod-name>
```

```bash
kubectl logs <pod-name>
```

```bash
kubectl exec -it <pod-name> -- /bin/bash
```

```bash
kubectl delete pod <pod-name>
```

---

## Deployments

```bash
kubectl create deployment nginx --image=nginx
```

```bash
kubectl get deployments
```

```bash
kubectl describe deployment nginx
```

```bash
kubectl scale deployment nginx --replicas=3
```

```bash
kubectl rollout status deployment nginx
```

```bash
kubectl rollout history deployment nginx
```

```bash
kubectl rollout undo deployment nginx
```

```bash
kubectl delete deployment nginx
```

---

## ReplicaSets

```bash
kubectl get rs
```

```bash
kubectl describe rs <replicaset-name>
```

---

## Services

```bash
kubectl get svc
```

```bash
kubectl describe svc <service-name>
```

```bash
kubectl delete svc <service-name>
```

---

## YAML Files

```bash
kubectl apply -f deployment.yaml
```

Create or update resources.

```bash
kubectl create -f deployment.yaml
```

Create only.

```bash
kubectl delete -f deployment.yaml
```

Delete resources.

---

## Config

```bash
kubectl config view
```

```bash
kubectl config current-context
```

```bash
kubectl config get-contexts
```

---

## Labels

```bash
kubectl get pods --show-labels
```

```bash
kubectl label pod nginx env=production
```

---

## Secrets

```bash
kubectl get secrets
```

```bash
kubectl create secret generic my-secret --from-literal=username=admin --from-literal=password=123456
```

---

## ConfigMap

```bash
kubectl get configmap
```

```bash
kubectl create configmap app-config --from-literal=color=blue
```

---

## Events

```bash
kubectl get events
```

---

## Resource Usage

```bash
kubectl top nodes
```

```bash
kubectl top pods
```

---

## Debugging

```bash
kubectl describe pod <pod-name>
```

```bash
kubectl logs <pod-name>
```

```bash
kubectl get events
```

---

## Delete Resources

```bash
kubectl delete pod <pod-name>
```

```bash
kubectl delete deployment <deployment-name>
```

```bash
kubectl delete service <service-name>
```

```bash
kubectl delete namespace <namespace-name>
```

---

# Useful Short Commands

| Command | Description |
|----------|-------------|
| `kubectl get po` | Pods |
| `kubectl get deploy` | Deployments |
| `kubectl get rs` | ReplicaSets |
| `kubectl get svc` | Services |
| `kubectl get ns` | Namespaces |
| `kubectl get all` | All Resources |
| `kubectl get pvc` | Persistent Volume Claims |
| `kubectl get pv` | Persistent Volumes |
| `kubectl get ingress` | Ingress |
| `kubectl get cm` | ConfigMaps |

---

# Most Used Commands

```bash
kubectl get all

kubectl apply -f file.yaml

kubectl delete -f file.yaml

kubectl logs <pod-name>

kubectl exec -it <pod-name> -- /bin/bash

kubectl describe pod <pod-name>

kubectl scale deployment nginx --replicas=3

kubectl rollout undo deployment nginx
```
