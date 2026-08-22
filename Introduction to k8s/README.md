<img src= "https://github.com/gauthamr58/Kubernetes-Zero-To-Hero/blob/main/Introduction%20to%20k8s/assets/evolution.png" alt="Banner"/>


## Why you need Kubernetes and what it can do
Before Kubernetes and containers became standard, software infrastructure went through two major phases

1:Bare-Metal physical servers 

Early on, organizations ran applications on physical servers. There was no way to define resource boundaries for applications in a physical server, and this caused resource allocation issues. For example, if multiple applications run on a physical server, there can be instances where one application would take up most of the resources, and as a result, the other applications would underperform. A solution for this would be to run each application on a different physical server. But this did not scale as resources were underutilized, and it was expensive for organizations to maintain many physical servers.

2: Virtual machines (VM's),

As a solution, virtualization was introduced. It allows you to run multiple Virtual Machines (VMs) on a single physical server's CPU. Virtualization allows applications to be isolated between VMs and provides a level of security as the information of one application cannot be freely accessed by another application.

Virtualization allows better utilization of resources in a physical server and allows better scalability because an application can be added or updated easily, reduces hardware costs, and much more.

### Container deployment era:
Containers are similar to VMs, but they have relaxed isolation properties to share the Operating System (OS) among the applications. Therefore, containers are considered lightweight. Similar to a VM, a container has its own filesystem, share of CPU, memory, process space, and more. As they are decoupled from the underlying infrastructure, they are portable across clouds and OS distributions.

Containers have become popular because they provide extra benefits, such as:

- Agile application creation and deployment: increased ease and efficiency of container image creation compared to VM image use.
- Continuous development, integration, and deployment: provides reliable and frequent container image build and deployment with quick and efficient rollbacks (due to image immutability).
- Dev and Ops separation of concerns: create application container images at build/release time rather than deployment time, thereby decoupling applications from infrastructure.
- Observability: not only surfaces OS-level information and metrics, but also application health and other signals.
- Environmental consistency across development, testing, and production: runs the same on a laptop as it does in the cloud.
- Cloud and OS distribution portability: runs on Ubuntu, RHEL, CoreOS, on-premises, on major public clouds, and anywhere else.
- Application-centric management: raises the level of abstraction from running an OS on virtual hardware to running an application on an OS using logical resources.
- Loosely coupled, distributed, elastic, liberated micro-services: applications are broken into smaller, independent pieces and can be deployed and managed dynamically – not a monolithic stack running on one big single-purpose machine.
- Resource isolation: predictable application performance.
- Resource utilization: high efficiency and density.

Containers are a good way to bundle and run your applications, docker is powerful for single instances,but this approach quickly hits severe limitations.

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