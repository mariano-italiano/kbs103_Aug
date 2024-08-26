# Installation procedure

1. Modules (overlay + br_netfilter)
2. Sysctl parameters
3. Containerd + required packages
4. Disable SWAP
5. Add K8s repository
6. Installing kubelet + kubectl + kubeadm (same version is required)
7. Initialize the K8s cluster
8. Install Network Plugin (CNI plugin/network addon)
9. Join worker nodes

Master node(s): 1-8
Worker node(s): 1-6, 9

Installation script: [deploy_k8s.sh](deploy_k8s.sh)
