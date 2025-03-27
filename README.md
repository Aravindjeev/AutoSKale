# **AutoSkale - Intelligent Kubernetes Autoscaler Monitor**








## **Overview**

AutoSkale is an intelligent Kubernetes autoscaling analysis tool designed to help DevOps teams monitor, analyze, and optimize Kubernetes Horizontal Pod Autoscaler (HPA) and Cluster Autoscaler performance. It provides deep insights into scaling behavior, detects anomalies, and suggests improvements to ensure efficient resource utilization across GKE, EKS, AKS, and on-prem clusters.

## Key Features 🚀

1. 📊 Real-time Autoscaler Monitoring – Fetch HPA & Cluster Autoscaler events dynamically.

2. 📈 Resource Utilization Insights – Track CPU, memory, and pod scaling trends.

3. ⚠️ Alerts & Notifications – Slack, Email, and Webhook-based alerts for scaling anomalies.

4. 📊 Grafana Dashboards – Visualize autoscaling trends and pod behaviors.

5. 🧠 AI-Powered Recommendations (Coming Soon) – Smart tuning suggestions for optimal autoscaling.

## Architecture

 +--------------------+        +----------------------+        +-------------------+
 | Kubernetes Cluster | ---> | AutoSkale API       | ---> | Prometheus / Grafana |
 +--------------------+        +----------------------+        +-------------------+
         |                           |                        |
         |                           |                        |
  Cluster Autoscaler        HPA Metrics           Alerts / Logs

## Getting Started

### Prerequisites

1. Python 3.8+

2. Kubernetes cluster (GKE, EKS, AKS, Minikube, etc.)

3. Helm & kubectl installed

5. Prometheus (for optional monitoring)

### Installation

1. Clone the Repository

``` 
git clone https://github.com/your-username/AutoSkale.git
cd AutoSkale 
```

2. Install Dependencies

`pip install -r requirements.txt`

3. Deploy AutoSkale in Kubernetes

`kubectl apply -f autoskale.yaml`

4. Run AutoSkale Locally

`python autoskale.py`

### Configuration

Modify the config/settings.yaml file to adjust scaling thresholds, alerting configurations, and monitoring settings.

```
scaling:
  cpu_threshold: 70
  memory_threshold: 80
  min_replicas: 2
  max_replicas: 10
```
## Roadmap 🛣️

For detailed upcoming features and milestones, check out our [ROADMAP.md](https://github.com/Aravindjeev/AutoSKale/blob/ce0329446ca8b8547c27ca12e606fa5944a78356/ROADMAP.md).

## Contributing 🤝

We welcome contributions! Please read our [CONTRIBUTING.md] for guidelines.

## License 📜

This project is licensed under the Apache 2.0 License. See the LICENSE file for details.

## Community & Support 💬

Slack: Join our community

GitHub Issues: Report a bug

CNCF SIG: Proposal Submission

🚀 **AutoSkale – Optimize Kubernetes Autoscaling Like a Pro!**

