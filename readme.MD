## Selectors
### Taint the node
```
kubectl taint nodes node1 Taintkey1=Taintvalue1:NoSchedule
kubectl taint nodes ip-192-168-23-73.ec2.internal hardware=gpu:NoSchedule
```
### UnTaint the node 
```
kubectl taint nodes node1 Taintkey1=Taintvalue1:NoSchedule-
```

### label nodes
```
kubectl label nodes <your-node-name> disktype=ssd
kubectl label nodes ip-192-168-23-73.ec2.internal hardware=gpu
```
Ref: https://kubernetes.io/docs/tasks/configure-pod-container/assign-pods-nodes/

### affinity
1. affinity means attraction

### antiaffinity
1. anti attraction

```
1. requiredDuringSchedulingIgnoredDuringExecution = Hard match
2. preferredDuringSchedulingIgnoredDuringExecution = Soft match
```

![alt text](podaffinityandpodantiaffinity.svg)