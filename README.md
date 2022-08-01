# Certified Kubernetes Application Developer-CKAD

## Exam Brief

- Duration : 2 hours
- Performance-Based Exam
- Certification validity: 3 years
- Prerequisite: None
- Cost: $395 USD, 1 year exam eligibility, with a free retake within the year.
- [Official KCNA curriculum](https://github.com/cncf/curriculum/blob/master/CKAD_Curriculum_v1.24.pdf)
  
### Useful keys & Common accronyms in Kubernetes

- K8s = Kubernetes
- CNCF = Cloud Native Computing Foundation
- NetPol = Network Policies
- PV = Persistent Volumes
- PVC = Persistent Volume Claims
- CSI = Container Storage Interface
- CNI = Container Network Interface
- CI/CD = Continuous Integration & Continuous Deployment
- RBAC = Role Based Access Control
- OCI = Open Container Initiative
- CRI = Container Runtime Interface
- SMI = Service Mesh Interface
- SLO = Service Level Objectives
- SLI = Service Level Indicators
- SLA = Service Level Agreements

## 1. Core concepts

### 1.2 Architecture

A cluster is formed by different nodes, where pods are deployed. The whole cluster
is managed by the master.

Kubernetes is composed by:

- API server: It is the component that allows us to comunicate with our cluster
- etcd: It is a key-value distributed store, it sotores data to manage our cluster
- kubelet: agent that runs on each node
- comtainer runtime: software to run containers
- controller: it orchestrait the cluster. If a node falls this component manage the situation
- scheduler: It asigns tasks to nodes

Pods and services only runs on workers, teh master nodes only manage the cluster and had the API server.

Our client aplication is kubectl, it allows us to interact with our cluster.
