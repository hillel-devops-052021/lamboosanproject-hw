# sergeykudelin-hw

minikube start -p first-cluster  - create first cluster

minikube start -p second-cluster - create second cluster

kubectl config get-contexts       - check status clusters

kubectl config use-context first-cluster - switch to first cluster

kubectl get ns - get namespace info

kubectl get nodes - get nodes info


minikube delete -p second-cluster - delete cluster

minikube ssh -p first-cluster - connect to first cluster


minikube addons enable csi-hostpath-driver -p first-cluster


kubectl apply -f pvc_mongo.yml persistentvolumeclaim/mongo-pvc created
