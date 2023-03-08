# EKS-Microservices-Deployment
Microservices Deployment on EKS 


PS C:\WINDOWS\system32> eksctl create cluster --name in28minutes-cluster --nodegroup-name in28minutes-cluster-node-group  --node-type t2.medium --nodes 3 --nodes-min 3 --nodes-max 7 --managed --asg-access
2023-03-08 13:03:50 [ℹ]  eksctl version 0.132.0
2023-03-08 13:03:50 [ℹ]  using region us-east-2
2023-03-08 13:03:51 [ℹ]  setting availability zones to [us-east-2a us-east-2b us-east-2c]
2023-03-08 13:03:51 [ℹ]  subnets for us-east-2a - public:192.168.0.0/19 private:192.168.96.0/19
2023-03-08 13:03:51 [ℹ]  subnets for us-east-2b - public:192.168.32.0/19 private:192.168.128.0/19
2023-03-08 13:03:51 [ℹ]  subnets for us-east-2c - public:192.168.64.0/19 private:192.168.160.0/19
2023-03-08 13:03:51 [ℹ]  nodegroup "in28minutes-cluster-node-group" will use "" [AmazonLinux2/1.24]
2023-03-08 13:03:51 [ℹ]  using Kubernetes version 1.24
2023-03-08 13:03:51 [ℹ]  creating EKS cluster "in28minutes-cluster" in "us-east-2" region with managed nodes
2023-03-08 13:03:51 [ℹ]  will create 2 separate CloudFormation stacks for cluster itself and the initial managed nodegroup
2023-03-08 13:03:51 [ℹ]  if you encounter any issues, check CloudFormation console or try 'eksctl utils describe-stacks --region=us-east-2 --cluster=in28minutes-cluster'
2023-03-08 13:03:51 [ℹ]  Kubernetes API endpoint access will use default of {publicAccess=true, privateAccess=false} for cluster "in28minutes-cluster" in "us-east-2"
2023-03-08 13:03:51 [ℹ]  CloudWatch logging will not be enabled for cluster "in28minutes-cluster" in "us-east-2"
2023-03-08 13:03:51 [ℹ]  you can enable it with 'eksctl utils update-cluster-logging --enable-types={SPECIFY-YOUR-LOG-TYPES-HERE (e.g. all)} --region=us-east-2 --cluster=in28minutes-cluster'
2023-03-08 13:03:51 [ℹ]
2 sequential tasks: { create cluster control plane "in28minutes-cluster",
    2 sequential sub-tasks: {
        wait for control plane to become ready,
        create managed nodegroup "in28minutes-cluster-node-group",
    }
}
2023-03-08 13:03:51 [ℹ]  building cluster stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:03:51 [ℹ]  deploying stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:04:21 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:04:51 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:05:52 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:06:52 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:07:52 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:08:52 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:09:53 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:10:53 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:11:53 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:12:53 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:13:53 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:14:54 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-cluster"
2023-03-08 13:16:56 [ℹ]  building managed nodegroup stack "eksctl-in28minutes-cluster-nodegroup-in28minutes-cluster-node-group"
2023-03-08 13:16:56 [ℹ]  deploying stack "eksctl-in28minutes-cluster-nodegroup-in28minutes-cluster-node-group"
2023-03-08 13:16:56 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-nodegroup-in28minutes-cluster-node-group"
2023-03-08 13:17:26 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-nodegroup-in28minutes-cluster-node-group"
2023-03-08 13:18:04 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-nodegroup-in28minutes-cluster-node-group"
2023-03-08 13:19:44 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-nodegroup-in28minutes-cluster-node-group"
2023-03-08 13:20:53 [ℹ]  waiting for CloudFormation stack "eksctl-in28minutes-cluster-nodegroup-in28minutes-cluster-node-group"
2023-03-08 13:20:53 [ℹ]  waiting for the control plane to become ready
2023-03-08 13:20:53 [✔]  saved kubeconfig as "C:\\Users\\taroseri\\.kube\\config"
2023-03-08 13:20:53 [ℹ]  no tasks
2023-03-08 13:20:53 [✔]  all EKS cluster resources for "in28minutes-cluster" have been created
2023-03-08 13:20:53 [ℹ]  nodegroup "in28minutes-cluster-node-group" has 3 node(s)
2023-03-08 13:20:53 [ℹ]  node "ip-192-168-38-191.us-east-2.compute.internal" is ready
2023-03-08 13:20:53 [ℹ]  node "ip-192-168-5-13.us-east-2.compute.internal" is ready
2023-03-08 13:20:53 [ℹ]  node "ip-192-168-71-81.us-east-2.compute.internal" is ready
2023-03-08 13:20:53 [ℹ]  waiting for at least 3 node(s) to become ready in "in28minutes-cluster-node-group"
2023-03-08 13:20:53 [ℹ]  nodegroup "in28minutes-cluster-node-group" has 3 node(s)
2023-03-08 13:20:53 [ℹ]  node "ip-192-168-38-191.us-east-2.compute.internal" is ready
2023-03-08 13:20:53 [ℹ]  node "ip-192-168-5-13.us-east-2.compute.internal" is ready
2023-03-08 13:20:53 [ℹ]  node "ip-192-168-71-81.us-east-2.compute.internal" is ready
2023-03-08 13:20:55 [ℹ]  kubectl command should work with "C:\\Users\\taroseri\\.kube\\config", try 'kubectl get nodes'
2023-03-08 13:20:55 [✔]  EKS cluster "in28minutes-cluster" in "us-east-2" region is ready
PS C:\WINDOWS\system32> kubectl get nodes
NAME                                           STATUS   ROLES    AGE   VERSION
ip-192-168-38-191.us-east-2.compute.internal   Ready    <none>   14m   v1.24.10-eks-48e63af
ip-192-168-5-13.us-east-2.compute.internal     Ready    <none>   14m   v1.24.10-eks-48e63af
ip-192-168-71-81.us-east-2.compute.internal    Ready    <none>   15m   v1.24.10-eks-48e63af
PS C:\WINDOWS\system32> kubectl create deployment hello-world-rest-api --image=taroserigano/hello-world-rest-api:0.0.1.RELEASE
deployment.apps/hello-world-rest-api created
PS C:\WINDOWS\system32> kubectl expose deployment hello-world-rest-api --type=LoadBalancer --port=8080
service/hello-world-rest-api exposed
PS C:\WINDOWS\system32> kubectl get deployment
NAME                   READY   UP-TO-DATE   AVAILABLE   AGE
hello-world-rest-api   0/1     1            0           47s
PS C:\WINDOWS\system32> kubectl get replicaset
NAME                             DESIRED   CURRENT   READY   AGE
hello-world-rest-api-b9b6b6544   1         1         0       81s
PS C:\WINDOWS\system32> kubectl get pod
NAME                                   READY   STATUS             RESTARTS   AGE
hello-world-rest-api-b9b6b6544-gbxfb   0/1     ImagePullBackOff   0          94s
PS C:\WINDOWS\system32> kubectl create deployment todowebapp-h2 --image=taroserigano/todo-web-application-h2:0.0.1-SNAPSHOT
deployment.apps/todowebapp-h2 created
PS C:\WINDOWS\system32> kubectl get svc
NAME                   TYPE           CLUSTER-IP      EXTERNAL-IP                                                               PORT(S)          AGE
hello-world-rest-api   LoadBalancer   10.100.140.27   a7370dd807deb4391904a5af5abcc50f-2118375849.us-east-2.elb.amazonaws.com   8080:31242/TCP   2m44s
kubernetes             ClusterIP      10.100.0.1      <none>                                                                    443/TCP          30m
PS C:\WINDOWS\system32> kubectl expose deployment todowebapp-h2 --type=LoadBalancer --port=8080
service/todowebapp-h2 exposed
PS C:\WINDOWS\system32>
PS C:\WINDOWS\system32>
PS C:\WINDOWS\system32>
PS C:\WINDOWS\system32>
