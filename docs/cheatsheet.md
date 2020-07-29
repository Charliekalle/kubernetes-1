List Master nodes
```
kubectl get nodes --selector='node-role.kubernetes.io/master'
```
List worker nodes
```
kubectl get nodes --selector='!node-role.kubernetes.io/master'
```
Reset k8s Cluster
ref: https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-reset/
```
kubeadm reset --force
```
Cluster join command
```
kubeadm token create --print-join-command
```
