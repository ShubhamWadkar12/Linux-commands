| Port | Protocol | Service / Tool | Usage |
|---|---|---|---|
| 22 | TCP | SSH | Remote Linux server administration. |
| 53 | TCP/UDP | DNS | Domain name resolution. |
| 80 | TCP | HTTP | Web server communication. |
| 443 | TCP | HTTPS | Secure web server communication. |
| 3000 | TCP | Grafana | Grafana dashboard (default). |
| 3000 | TCP | Node.js | Common development application port. |
| 3306 | TCP | MySQL | MySQL database connections. |
| 5432 | TCP | PostgreSQL | PostgreSQL database connections. |
| 6379 | TCP | Redis | Redis cache/database connections. |
| 6443 | TCP | Kubernetes API Server | Kubernetes cluster API communication. |
| 8080 | TCP | Jenkins | Jenkins web interface (default). |
| 8080 | TCP | HTTP Alternate | Common application server port. |
| 8443 | TCP | HTTPS Alternate | Alternative secure web interface. |
| 9090 | TCP | Prometheus | Prometheus monitoring interface and API (default). |
| 9093 | TCP | Alertmanager | Prometheus Alertmanager web interface (default). |
| 9100 | TCP | Node Exporter | Linux server metrics for Prometheus (default). |
| 10250 | TCP | Kubelet | Kubernetes node management API. |
| 10257 | TCP | kube-controller-manager | Kubernetes controller manager health and metrics endpoint (default). |
| 10259 | TCP | kube-scheduler | Kubernetes scheduler health and metrics endpoint (default). |
| 2375 | TCP | Docker API | Docker remote API without TLS. |
| 2376 | TCP | Docker API | Docker remote API with TLS. |
| 2379 | TCP | etcd | Kubernetes cluster key-value store client communication. |
| 2380 | TCP | etcd | etcd peer communication. |
| 30000–32767 | TCP/UDP | Kubernetes NodePort | Exposes Kubernetes services through node ports. |
| 5000 | TCP | Docker Registry | Common private container registry port. |
| 50000 | TCP | Jenkins Agent | Common inbound agent port when configured. |
| 9200 | TCP | Elasticsearch | Elasticsearch HTTP API (default). |
| 9300 | TCP | Elasticsearch | Elasticsearch node-to-node transport (default). |

**Important:** Port numbers shown are common defaults. Actual ports may vary depending on application configuration and deployment.
