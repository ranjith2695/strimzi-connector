Creating a PostgreSQL DB using kubectl

kubectl apply -f postgres-config.yaml 

kubectl apply -f postgres-pvc-pv.yaml

kubectl apply -f postgres-deployment.yaml

kubectl apply -f postgres-service.yaml 

kubectl get pods

kubectl exec -it postgres-6c9b6585d4-756qb --  psql -h postgres -U test --password -p 5432 demo


