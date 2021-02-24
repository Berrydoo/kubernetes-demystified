Kubernetes Demystified

Outline:
1. What is it 
1. What's in a cluster
1. Interacting with it
   1. kubectl ( mention kubeconfig )
   		1. get pods, -w, --show-labels, --all-namespaces, -o 
   		1. get svc
   		1. get all / get pods,svc 
   1. yaml file walkthrough ( py charm )
   1. Lens app
1. Resources / Resource types 
   1. kubectl api-resources 
   1. pod
   1. deployment
   1. service
   1. configmap
   1. secret
   1. namespace
1. What if something goes wrong?
   1. logs
   1. describe
   1. get events
   1. exec 
   1. kubectl top pods --containers
1. frickin helpful commands
   1. kubectl api-resources
   1. kubectl explain pod --recursive | less 
   1. alias k=kubectl
   1. output related
      1. -o wide
      1. -o yaml
      1. -o json
      1. --all-namespaces or -A
      1. get all
      1. get pods --show-labels 
1. gotchas
   1. no tab characters
   1. no jvm memory flags - let kubernetes control the memory 
1. getting help
   1. kubernetes documentation
   1. kubectl create --help
   1. kubectl explain pod --recursive | less





Lab

- write a blog about sports
create a pod that shows a web page

- we need a new image 
delete the pod 
update the yaml file  
apply the changes

- add a new container to a pod
add a container to log output
look at the logs from the console
exec into the pod to show a mounted volume

- our traffic is heavy, so replace the pod with a deployment
create a deployment
delete a pod and watch it get rebuilt
show rollout history
update the image with an error and watch what happens
use describe to see errors
get events to see errors
rollback the deployment
fix the error and rollout a new version


Should we cover?
- liveness / readiness probes 
- namespaces
- undestand resources - Mi, milli-cpus
- volumes

Game plan
- first session to do powerpoint
- second to do a lab 
- Use Docker Desktop for users to experiment 


