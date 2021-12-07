# DevOps-Challenge 
## Workflow
* I followed this blog to dockerize a sample app (ruby-on-rails-app), link: https://semaphoreci.com/community/tutorials/dockerizing-a-ruby-on-rails-application.
* Test the stack by running the following command: ```$ docker-compose up``` 
* Start making kubernetes manifests by making ```env-configmap.yml``` file to pass the enviromment variables.
* Create ```drkiq.yml``` file that includes deployment & service for drkiq app
* Create ```postgres.yml``` file that includes deployment & service for postgres app
* Create ```postgres-pvc.yml``` file that includes persistent volume claim for postgres app
* Create ```redis.yml``` file that includes deployment & service for redis app
* Create ```redis-pvc.yml``` file that includes persistent volume claim for redis app
* Create ```sidekiq.yml``` file that includes deployment for sidekiq app 
* Create ```nginx.yml``` file that includes deployment & service for redis app, note: i made this app an external service with nodePort: 30000
## Cluster test
* Start creating the cluster using Play with Kubernetes platform link: https://labs.play-with-k8s.com/
* Create all kubernetes manifests using the following command: ```$ kubectl apply -f <file name>```
* Check for all objects with the following command: ```$ kubectl get all``` 
