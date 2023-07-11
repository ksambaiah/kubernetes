# Kubernetes Components

There are broadly two components we have in kubernetes.

 - Control Panel
 - Kubernetes

## Control Panel

Control panel broadly divided into the following:

 - API Server
 - Control Manager
 - Scheduler
 - etcd
API Server:  This is the component you interact with the kubernetes always. It is kind of orchestration for all components. You can interact with curl (cumberson) or using kubctl cli.
etcd: etcd is key value store which is central to Kubernetes. You need to start etcd first and tell API server about etcd service.
Control Manager: It consists of multiple components which interacts with apiserver and writes to etcd.
Scheduler: Scheduler is responsible to assiging pods to different nodes (here assign doesn't mean it tells which node to pick which pod, Scheduler write the information to etcd).

## Nodes

Nodes will be running

 - Kubelet
 - kube-proxy
 - Kubelet interacts with api server and gets the required pods to run on it.
 - Kube-prox This is very important component responsible for managing iptables on the node.

## Interaction of components

![enter image description here](./K8S-Architecture.png)


## Links to architecture of Kubernetes

[Excellent link explaining architecutre](https://www.youtube.com/watch?v=3KtEAa7_duA)
[Kubernetes bootcamp ](https://github.com/jungho/k8s-bootcamp/tree/master)
