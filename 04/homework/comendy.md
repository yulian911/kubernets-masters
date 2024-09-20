instalacja ingresa w chmurze:

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.5.1/deploy/static/provider/cloud/deploy.yaml

kubectl get pods -n [name_namespace] name=ingress-nginx --watch

kubectl get svc --namespace=[name_namespace]

czyszvczenie

kubectl delete -f ingress-resource.yml
kubectl delete -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.5.1/deploy/static/provider/cloud/deploy.yaml

kubectl delete -f [plik deployu].yaml -f [plik servisu].yaml

tworzenie namespace
kubectl create namespace [nazwa]

kubectl get ingress -A -sprawdzenie ingresu

kubectl port-forward my-pod-name 8080:8080

kubectl apply -f i .\zawarosc folderu - caly folder zapuszcza
kubectl delete -f i .\zawarosc folderu - caly folder usuwa

kubectl describe pod two-containers - opis poda
