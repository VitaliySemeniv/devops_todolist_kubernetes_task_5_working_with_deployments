kubectl apply -f .infrastructure/namespace.yml       # якщо потрібно
kubectl -n mateapp apply -f .infrastructure/deployment.yml
kubectl -n mateapp apply -f .infrastructure/hpa.yml
kubectl -n mateapp rollout status deploy/todoapp
