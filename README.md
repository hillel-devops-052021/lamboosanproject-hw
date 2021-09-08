# sergeykudelin-hw

minikube start -p first-cluster  - create first cluster

minikube addons enable csi-hostpath-driver -p first-cluster  -  enable CSI module in cluster

kubectl apply -f pvc_mongo.yml - create persistent volumes for pvc_mongo

kubectl apply -f statefulset_mongo.yml - create StatefulSets recourses

kubectl apply -f svc_mongo.yml  - create "network" service for mongo pods

kubectl apply -f deployment_backend.yml  - deploy backend

kubectl apply -f deployment_frontend.yml - deploy frontend

minikube addons enable ingress -p first-cluster  -  enable Ingress module in cluster

kubectl apply -f svc_frontend.yml - create "network" service for frontend pods

kubectl apply -f svc_backend.yml  - create "network" service for backend pods

kubectl apply -f ingress_frontend.yml  - create ingress for frontend pods

kubectl apply -f ingress_backend.yml  - create ingress for backend pods

minikube ip -p first-cluster - get cluster IP address

add IP address and DNS name to resolv.conf

kubectl apply -f deployment_admin_mongo.yml - deploy mongo admin panel

kubectl apply -f svc_mongo_admin.yml  - create "network" service for mongo admin panel
