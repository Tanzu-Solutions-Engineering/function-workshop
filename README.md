Functions Workshop
=====================

This workshop covers the various options for deploying functions in Tanzu Application Platform 1.2.

## Pre-requisistes
- A Kubernetes cluster with Tanzu Application Platform installed with the "Full" profile, or at least the following packages:
  -  The [Learning Center package](https://docs.vmware.com/en/VMware-Tanzu-Application-Platform/1.2/tap/GUID-learning-center-install-learning-center.html)
  -  The [Functions (Beta) functionality](https://docs.vmware.com/en/VMware-Tanzu-Application-Platform/1.2/tap/GUID-workloads-using-functions.html)
  -  The [Cloud Native Runtimes package](https://docs.vmware.com/en/VMware-Tanzu-Application-Platform/1.2/tap/GUID-cloud-native-runtimes-install-cnrt.html)

## Install
To deploy and view this sample workshop, run:

```
kubectl apply -f https://raw.githubusercontent.com/Tanzu-Solutions-Engineering/function-workshop/main/resources/workshop.yaml
kubectl apply -f https://raw.githubusercontent.com/Tanzu-Solutions-Engineering/function-workshop/main/resources/training-portal.yaml
```

This will deploy a training portal hosting just this workshop. To get the
URL for accessing the training portal run:

```
kubectl get trainingportal/lab-markdown-sample
```

The training portal is configured to allow anonymous access. For your own
workshop content you should consider removing anonymous access.
