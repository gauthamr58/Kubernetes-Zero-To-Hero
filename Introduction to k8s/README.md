<img src= "https://github.com/gauthamr58/Kubernetes-Zero-To-Hero/blob/main/Introduction%20to%20k8s/assets/evolution.png" alt="Banner"/>


## Why you need Kubernetes and what it can do
Before Kubernetes and containers became standard, software infrastructure went through two major phases

1:Bare-Metal physical servers 

2: Virtual machines (VM's),

and then conatainers came and Containers are a good way to bundle and run your applications, docker is powerful for single instances,but this approach quickly hits severe limitations.

Kubernetes can and provides you with:

- **Automates Scaling:** Scale your application up and down with a simple command, with a UI, or automatically based on CPU usage.
- **Self-Healing:** Automatically restarts failed containers, replaces unhealthy ones, and moves containers from failing nodes.
- **Service discovery:** Kubernetes can expose a container using a DNS name or its own IP address.
- **Load Balancing:** Distributes network traffic efficiently across all healthy instances of your application.
- **Automated Rollouts & Rollbacks:** Manages the rollout of new versions, allowing for zero-downtime updates and easy reversion if issues arise.
- **Resource Management:** Allows you to define resource requests and limits for your containers, ensuring fair resource allocation.
- **Centralized Configuration & Secret Management:** Provides secure ways to inject configuration data and sensitive information into your containers.
- **Declarative Configuration:** You describe the desired state of your applications (e.g., "I want 3 instances of my web app running"), and Kubernetes works to maintain that state, continuously monitoring and correcting deviations.








## What is kubernetes?
Kubernetes (often abbreviated as **K8s**) is an open-source container orchestration platform designed to automate the deployment, scaling, and management of containerized applications. Originally developed by Google and now maintained by the Cloud Native Computing Foundation (CNCF), it serves as the operating system for cloud-native infrastructure, and providing a consistent environment for your applications, no matter where they run (on-premises, public cloud, hybrid cloud).