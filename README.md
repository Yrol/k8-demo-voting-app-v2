## A simple voting app running on K8s.
A voting and results app that can be deployed on a K8s cluster using deployement scripts. This consist of following services
- PostgreSQL
- Redis
- Voting app (front-end) - type: LoadBalancer
- Result app (front-end) - type: LoadBalancer

In addition to that, a worker app also included (`worker-app-deployment.yml`) to capture votes from temporary Redis services to PostGres DB

### How to deploy
```
kubectl create -f .
```