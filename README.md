Cloud Native DevOps with Kubernetes (2019)

```
vi main.go
vi Dockerfile

docker build -t myhello .
docker run -p 9999:8888 -d myhello
docke ps
docker rm -f <container_id>

docker login
docker image tag myhello reisinge/myhello
docker image push reisinge/myhello

kubectl run demo --image=reisinge/myhello --port=9999 --labels app=demo
kubectl port-forward deploy/demo 9999:8888
kubectl get pods --selector app=demo
```
