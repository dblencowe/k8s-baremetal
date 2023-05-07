# K8S Baremetal Playbook

Ansible Playbook for deploying a Kubernetes Cluster to baremetal hardware

The playbook accomplishes several basic tasks for setting up a Cluster:
- Configure Nodes
- - Enable cgroups for Raspberry Pis
- Create cluster on Kubernetes Master
- Join worker nodes to the cluster
- Install Core Applications
- - MetalLB - Service / LoadBalancer external IP provisioning
- - Longhorn - synchronised file storage on nodes
- - External DNS (optional) - Publish DNS records for external services
