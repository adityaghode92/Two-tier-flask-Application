# How to setup two-tier application deployment on kubernetes cluster
## First setup kubernetes kubeadm cluster

## SetUp
- First clone the code to your machine
```bash
git clone https://github.com/Adityaghode92/Two-tier-flask-Application.git
```
- Move to k8s directory
```bash
cd two-tier-flask-app/k8s
```
- Now, execute below commands one by one
```bash
kubectl apply -f twotier-deployment.yml
```
```bash
kubectl apply -f twotier-deployment-svc.yml
```
```bash
kubectl apply -f mysql-deployment.yml
```
```bash
kubectl apply -f mysql-deployment-svc.yml
```
```bash
kubectl apply -f persistent-volume.yml
```
```bash
kubectl apply -f persistent-volume-claim.yml
```
