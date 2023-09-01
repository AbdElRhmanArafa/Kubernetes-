# Tasks Kubernetes

## Task 1: Install Minikube

Before you can start using Kubernetes, make sure you have Minikube installed. If not, you can follow the official documentation to [install Minikube](https://minikube.sigs.k8s.io/docs/start/) or docker desktop => (Enable Kubernetes option) .

## Task 2: Create a Redis Pod

To create a Redis Pod, use the appropriate `kubectl` command.

```bash
    kubectl run redis --image=redis
    kubectl get pods
```

## Task 3: Create an Nginx Pod

Create an Nginx Pod using a Pod definition YAML file. Create a file named `nginx-pod.yaml` with the necessary content, image Name should be nginx123.

```text
This will raise error ImagePullBackOff.
```

## Task 4: Check Nginx Pod Status

To check the status of the Nginx Pod, use the **kubectl get pod** command.

## Task 5: Change Nginx Pod Image

Change the Nginx Pod image to "nginx" using the appropriate `kubectl` command.

``` bash
kubectl set image pod/nginx nginx=nginx
kubectl edit pod nginx
```

## Task 6: Count ReplicaSets

To count how many ReplicaSets exist on the system, use the **kubectl get replicaset** command.

## Task 7: Create a ReplicaSet

Create a ReplicaSet with the specified name, image, and replicas using a YAML definition file.

``` bash
Pod status will be  CrashLoopBackOff
```

## Task 8: Scale ReplicaSet

Scale the specified ReplicaSet to a certain number of PODs using the **kubectl scale replicaset replica-set-1 --replicas=5** command.

## Task 9: Check READY Pods in ReplicaSet

To check how many PODs are READY in a specific ReplicaSet, use the appropriate `kubectl` command.

## Task 10: Delete a POD in ReplicaSet

Delete one of the PODs in a ReplicaSet using the `kubectl delete pod` command and observe the changes in the ReplicaSet.

## Task 11: Count Deployments and ReplicaSets

To count how many  ReplicaSets exist on the system, use the `kubectl get replicaset` command.

## Task 12: Create a Deployment

Create a Deployment with the specified name, image, and replicas using a YAML definition file.

## Task 13: Count Deployments and ReplicaSets (Again)

To count how many Deployments and ReplicaSets exist now, use the `kubectl get deployment,replicaset` command.

## Task 14: Check READY Pods in Deployment

To check how many PODs are ready in a specific Deployment, use the appropriate `kubectl` command.

## Task 15: Update Deployment Image

Update the image of a Deployment using the `kubectl set image` command and observe the changes in PODs.

## Task 16: Describe Deployment

Use the `kubectl describe deployment` command to inspect a Deployment and check the deployment strategy used for upgrading.

## Task 17: Rollback Deployment

Rollback a Deployment to a previous state using the appropriate `kubectl` command.

## Task 18: Create Nginx Deployment

Create a Deployment with specific settings, including labels, replicas, and container name, using a YAML definition file.

These tasks are designed to help you practice various operations in a Kubernetes cluster using `kubectl` and Minikube.
