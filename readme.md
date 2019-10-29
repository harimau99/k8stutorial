**Minikube - The local K8 in your laptop**
--
**For local that use minikube:**
minikube service `<deployment-name>`

--
**Viewing the Kubernetes in glance**

**To view running k8:**
kubectl get nodes

**To view deployment**
kubectl get deployments

**To view pods:**
kubectl get pods

**To view all pods/deployment:**
kubectl get all

**Check services:**
kubectl get services

**To check replica sets:**
kubectl get rs

--
**For label
Check pods label:**
Kubectl get pods  --show-labels

**Overwrite method:**
Kubectl label pod/<pods name>  app=<new label name> --overwrite

**To delete label:**
kubectl label pod/<pods name> app-

**Search through pods label**
--

**search pods label kubectl get pods -l `<label-name>`**
eg: kubectl get pods -l env=production
kubectl get pods -l env=production

Search pods label with selector. kubectl get pods --selector `<label-name1>,<label-name2>`

kubectl get pods --selector dev-lead=jim,env=production

**Deployment**
--

**To run K8 Applications and creating image**
kubectl run hw --image=karthequian/helloworld --port=80

**To create k8 with YAML Deployment file:**
kubectl create -f <name of yaml file>

**Expose the application:**
kubectl expose deployment hw --type=NodePort


