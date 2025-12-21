# Week 7: Content Delivery & Integration

## 🎯 Goal
Learn how to deliver content globally and decouple application components.

## 📚 Topics

### 1. Content Delivery
- **CloudFront**: CDN (Content Delivery Network). Caches content at Edge Locations.
    - S3 Origin vs Custom Origin.
    - OAI (Origin Access Identity) for S3 security.
- **Route 53**: Managed DNS Service.
    - Routing Policies: Simple, Weighted, Latency, Failover, Geolocation.

### 2. Application Integration
- **SQS (Simple Queue Service)**: Decouple and scale microservices, distributed systems, and serverless applications.
    - Standard vs FIFO.
- **SNS (Simple Notification Service)**: Pub/Sub messaging.
- **EventBridge**: Serverless event bus (formerly CloudWatch Events).

## 💡 Key Point
Decoupling is a major theme. SQS is often the answer to "loose coupling".
