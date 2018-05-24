#Kubernetes

[**Kubernetes**](https://kubernetes.io/) is a production grade constainer orchestration manager for automated container deployment, scaling and management.

## Overview of kubernetes

A kubernetes cluster is a collection of **Nodes**; where a node is a physical or virtual machine.

####Components
* **Master components**
	* **kube-apiserver** - exposes k8s API, front-end to control plane
	* **etcd** - HA key-value store, stores all k8s cluster data
	* **kube-scheduler** - assigns nodes to newly created pods in the cluster.
	* **kube-controller-manager** - runs controllers like Node controller, Service controller, Replication controller, Endpoints controller, Service Account and Token controllers.
	* **cloud-controller-manager** - interacts with underlying cloud providers.
* **Node components**
	* **kubelet** - agent which ensures that the pod state matches the podspec, i.e: The cluster state matches the desired state. Doesn't manage containers that were not create by k8s.
	* **kube-proxy** - enables service abstraction by maintianing network rules on the host and performing connection forwarding.
	* **container runtine** - responsible for running containers eg: docker, rkt, runc etc.,
* **Addons**
	* **DNS** - [**Cluster DNS**](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/) is required. DNS server which serves DNS records for k8s services.
	* Web UI (**Dashboard**)
	* [**Container resource monitoring**](https://kubernetes.io/docs/tasks/debug-application-cluster/resource-usage-monitoring/)
	* [**Cluster level logging**](https://kubernetes.io/docs/concepts/cluster-administration/logging/).
	* There are several other [**addons**](https://kubernetes.io/docs/concepts/cluster-administration/addons/) available.

####Installing a Highly available cluster

* Prerequisites
* Installing client tools
* Preparing the compute hosts
* generating TLS certificates
* 

