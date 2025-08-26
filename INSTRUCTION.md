kubectl -n mateapp delete -f .infrastructure/hpa.yml
kubectl -n mateapp delete -f .infrastructure/deployment.yml
# (опційно) якщо створювали:
kubectl -n mateapp delete -f .infrastructure/service.yml
kubectl -n mateapp delete -f .infrastructure/service-nodeport.yml
kubectl delete ns mateapp
