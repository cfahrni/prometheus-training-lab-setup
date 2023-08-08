# Prometheus lab setup

WIP repository for prometheus lab user setup:

Setup the namespaces with:

kubectl create namespace user1-monitoring
kubectl create namespace user1-monitoring-demo

helm -n user1-monitoring install user1-monitoring ./user-monitoring --set user=user1
helm -n user1-monitoring-demo install user1-monitoring-demo ./user-monitoring-demo --set user=user1


