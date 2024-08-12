# maybank

# useful commands

kubectl create -f namespace.yaml
kubectl create -f secret.yaml

kubectl create -f config-map.yaml
kubectl get cm -o yaml -n maybank | grep some

kubectl create -f storage.yaml

kubectl create -f deployment.yaml
kubectl delete deploy maybank-deployment -n maybank
kubectl exec <pod-name> -it /bin/sh -n maybank

kubectl create -f service.yaml

kubectl create -f ingress.yaml
sudo vi /private/etc/hosts
<minkube ip>  maybank-web-app.local

kubectl create -f horizontal_scaling.yaml
kubectl get hpa -n maybank




