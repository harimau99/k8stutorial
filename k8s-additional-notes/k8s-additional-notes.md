kubectl run hw --image karthequian/helloworld:latest
# This change from default deployment into red with label of hw

kubectl create -f blue.yml -f green.yml

kubectl apply -f sample-infrastructure.yml
#Applying sample sets.


