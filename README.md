# deploying-Kubernetes-statefulset-on-amazon-eks-multi-az

Stateful applications require consistent identity, ordered deployment, and persistent storage — all of which are hard to manage using traditional Kubernetes Deployment objects. This walkthrough focuses on StatefulSet, Kubernetes’ built-in controller to handle such requirements, especially for workloads like MySQL, Kafka, Redis, and Elasticsearch.

In this demo, we deploy a production-aligned MySQL StatefulSet on an Amazon EKS cluster spread across three availability zones. The setup uses Amazon EBS via CSI driver, gp3 volumes, and ensures fault-tolerant scheduling via pod anti-affinity. Each concept, from volume binding to pod rescheduling, is demonstrated with concrete steps and explanations.
