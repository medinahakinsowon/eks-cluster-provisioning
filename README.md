This is to upgrade your cluster using terraform aws module


The Amazon VPC CNI plugin for Kubernetes is the networking plugin for Pod networking in Amazon EKS clusters. The plugin is responsible for allocating VPC IP addresses to Kubernetes nodes and configuring the necessary networking for Pods on each node.


To access the cluster you have to authenticate

aws eks update-kubeconfig --name codemed-cluster --region us-east-1

Now the access your cluster
kubectl get nodes

Now deploy your app into the cluster---
kubectl apply -f deployment.yml

Now access the app-----
kubectl get svc


