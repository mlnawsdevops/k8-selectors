## Selectors
### Taint the node
```
kubectl taint nodes node1 Taintkey1=Taintvalue1:NoSchedule
kubectl taint node ip-192-168-23-73.ec2.internal hardware=gpu:NoSchedule
```