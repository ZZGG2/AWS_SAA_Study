# Week 5: Database

## 🎯 Goal
Distinguish between SQL and NoSQL, and understand scaling strategies.

## 📚 Topics

### 1. RDS (Relational Database Service)
- **Multi-AZ**: For Disaster Recovery (High Availability).
- **Read Replica**: For Performance (Read Scaling).

### 2. Aurora
- AWS native relational database.
- Serverless options.

### 3. DynamoDB (NoSQL)
- **Partition Key**: Determines data distribution.
- **GSI (Global Secondary Index)**: Index with different partition key.
- **LSI (Local Secondary Index)**: Index with same partition key but different sort key.

### 4. ElastiCache
- **Redis**: Advanced data structures, persistence, Multi-AZ.
- **Memcached**: Simple object caching, multi-threaded.

## 💡 Key Point
"Read Scaling vs Write Scaling". Almost guaranteed to be on the exam.
