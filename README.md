# AKS-Construct-Me-An-Amazing-Cluster-Config
A verbosely named repo where I'll be detailing an approach to Cluster Configs

## Dedicated or Shared

Its always a hard decision to make. Lots of small clusters of fewer big ones. 
I feel that Blast Radius is such an important operational aspect that i usually err towards smaller clusters. They need to be big enough to be mostly utilised, and spread over a number of zones, but if a single application meets those demands (say 6 nodes, with good pod density) then i would consider that a-ok.
For anything smaller than 6 nodes in the user pool, i'd say a shared cluster is going to be a better fit for these smaller apps.

## Stateful or stateless

## The cool k8s toys

Capability | Provided by | Managed ? 
---------- | ----------- | ---------
Autoscaling | KEDA | Y
Ingress
Service Mesh | Istio | Y
Network Policy | Cilium | Y
Network Provider | Azure CNI with Cilium | Y

## The surrounding infrastructure

Azure FrontDoor
