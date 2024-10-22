instalacja ingresa w chmurze:

instalacja ingresa na cloud
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.5.1/deploy/static/provider/cloud/deploy.yaml

kubectl get pods -n ingress-nginx name=ingress-nginx --watch

kubectl get svc --namespace=ingress-nginx

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

kubectl get pods -l app=redis-cluster -o jsonpath='{range.items[*]}{.status.podIP}:6379 '

kubectl exec -it redis-cluster-0 -- sh

redis-cli --cluster create --cluster-replicas 1 <TU WSTAWIĆ ADRESY IP WSZYSTKICH PODÓW>
kubectl exec -it redis-cluster-0 -- redis-cli cluster info

kubectl cluster-info - sprawdzenie kalastera
wygenerowanie certyfikatu

kubectl get configmap -n default kube-root-ca.crt -o jsonpath="{['data']['ca\.crt']}"

wygenerowanie tokena

kubectl create token gitlab -n kube-system

do sprawdzania endpointów placzyen z backendem:
kubectl get endpoints [api-service (nazwa serwisu backendu)]

helm create [nazwa]

sprawdzenie develpmentu 
kubectl logs -l name:api
