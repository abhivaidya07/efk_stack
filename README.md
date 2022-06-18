# deploysment of EFK stack on Kubernetes Cluster

1. [namespace.yaml](./namespace.yaml) - This yaml file creates a `kube-logging` namespace.
2. [elasticsearch_service.yaml](./elasticsearch_service.yaml) - This yaml file creates a headless service for the `elasticsearch` cluster.
3. [elasticsearch_statefulset.yaml](./elasticsearch_statefulset.yaml) - This yaml file deploys `elasticsearch` cluster in `kube-logging` namespace.
4. [kibana.yaml](./kibana.yaml) - This yaml file deploys `kibana` in the `kube-logging` namespace.
5. [fluentd.yaml](./fluentd.yaml) - This yaml file deploys `fluentd` daemonset in the `kube-logging` namespace.
6. [httpd.yaml](./httpd.yaml) - This yaml file creates a `httpd` namespace and deploys `httpd` web-server with an External-IP address.