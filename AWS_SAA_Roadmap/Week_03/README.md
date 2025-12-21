# Week 3: Compute

## 🎯 Goal
Understand the backbone of AWS compute services.
"Architecture diagrams start to appear here."

## 📚 Topics

### 1. EC2 (Elastic Compute Cloud)
- **Instance Types**: General Purpose, Compute Optimized, Memory Optimized, etc.
- **EBS vs Instance Store**: Persistent vs Ephemeral storage.

### 2. Scaling & Load Balancing
- **Auto Scaling Group (ASG)**: Automatically adjust the number of instances.
- **Elastic Load Balancer (ELB)**: Distribute incoming traffic.
    - **ALB (Application)**: Layer 7 (HTTP/HTTPS).
    - **NLB (Network)**: Layer 4 (TCP/UDP), High Performance.
    - **CLB (Classic)**: Legacy.

### 3. Placement Groups
- **Cluster**: Low latency, single AZ.
- **Spread**: Critical instances, distinct hardware.
- **Partition**: Distributed workloads (Hadoop, Kafka).

## 💡 Key Point
Understand when to use which Load Balancer and how Auto Scaling works with it.
