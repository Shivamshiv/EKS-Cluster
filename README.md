## Deploying Wordpress and MySQL on AWS EKS Cluster
*Deploying Wordpress(frontend) and MySQL(backend) on different pod/environment(Operating System) on AWS Elastic Kubernetes Services. Kubernetes deployments manage stateless services running on the cluster. Their purpose is to keep a set of identical pods running and upgrade them in a controlled way – performing a rolling update by default.*

### AWS EKS
- Amazon EKS (Elastic Kubernetes Service) is a managed Kubernetes service that allows you to run Kubernetes on AWS without the hassle of managing the Kubernetes control plane. 
- EKS is a managed containers-as-a-service (CaaS) that drastically simplifies Kubernetes deployment on AWS. 
- The big benefit of EKS, and other similar hosted Kubernetes services, is taking away the operational burden involved in running this control plane. You deploy cluster worker nodes using defined AMIs and with the help of CloudFormation, and EKS will provision, scale and manage the Kubernetes control plane for you to ensure high availability, security and scalability.

## Amazon EKS: Two Main Components
- **Control Plane:** The Control Plane consists of differnt Kubernetes master nodes that run in different availability zones (AZs). All incoming traffic to Kubernetes API comes through the network load balancer (NLB). It runs on the virtual private cloud controlled by Amazon. Hence, the Control Panel can’t be managed directly by the organization and is fully managed by AWS.
- **Worker Nodes:** Worner Nodes run on the Amazon EC2 instances in the virtual private cloud controlled by the organization. Any instance in AWS can be used as a worker node. These worker nodes can be accessed through SSH or provisioned without automation.

## Kubernetes
- Kubernetes is an open-source system that allows organizations to deploy and manage containerized applications like platforms as a service (PaaS), batch processing workers, and microservices in the cloud at scale. Through an abstraction layer created on top of a group of hosts, development teams can let Kubernetes manage a host of functions--including load balancing, monitoring and controlling resource consumption by team or application, limiting resource consumption and leveraging additional resources from new hosts added to a cluster, and other workflows.
- Through Amazon EKS, organizations using AWS can get the full functions of Kubernetes without having to install or manage Kubernetes itself.

