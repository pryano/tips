# Kubernetes
This is more of a cheat sheet of common kube commands.

* kubectl get pods   // show all deployed pods
* kubectl get pods --watch // show all deployed pods and updates as they happen
* kubectl get pods -n namespace-name // show all pods in the given namespace
* kubectl describe pod my-pod-name-3jak8 // show the details of the given pod
* kubectl delete pod my-pod-name-3jak8
* kubectl logs my-pod-name-3jak8 // show the standard output for the given pod
* kubectl get jobs
* kubectl delete job my-job-name // delete the job
