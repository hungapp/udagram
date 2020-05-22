# kubernetes

## Tasks

Set up K8s environment with kubectl and aws cli:
\$ aws eks --region <region_name> update-kubeconfig --name <cluster_name>

Create ConfigMaps from env files:
$ kubectl create configmap env-config --from-file=env-config.yml
$ kubectl create configmap env-secret --from-file=env-secret.yml
