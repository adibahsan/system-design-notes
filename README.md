# system-design-notes
A repository consists of my notes for system designing. Home notes are handwritten, some have been scrapped from the internet &amp; some are simply AI generated.

# Interview Tip (System Design) 📖💼

System design rounds are very common these days. Not only FAANG/MAANG companies, but many other organizations also take system design rounds very seriously.

Follow **Arun Kumar Singh** for more system design and interview tips.

The system design process is complex, and **one design doesn't fit all**. Below are useful rules to help you during an interview:

1. **For a Read-Heavy System** - Consider using a **Cache**.
2. **For a Write-Heavy System** - Use **Message Queues** for async processing.
3. **For Low Latency Requirements** - Consider using a **Cache** and **CDN**.
4. **Need Atomicity, Consistency, Isolation, Durability (ACID) compliance** - Use an **RDBMS/SQL Database**.
5. **Have unstructured data** - Opt for a **NoSQL Database**.
6. **For complex data (videos, images, files)** - Use **Blob/Object storage**.
7. **Complex pre-computation** - Leverage **Message Queues** & **Cache**.
8. **High-Volume Data Search** - Use **search index, tries, or search engines**.
9. **Scaling SQL Databases** - Implement **Database Sharding**.
10. **High Availability, Performance, and Throughput** - Use a **Load Balancer**.
11. **Global Data Delivery** - Consider using a **CDN**.
12. **Graph data (nodes, edges, relationships)** - Utilize a **Graph Database**.
13. **Scaling various components** - Implement **Horizontal Scaling**.
14. **High-performing database queries** - Use **Database Indexes**.
15. **Bulk Job Processing** - Consider **Batch Processing** & **Message Queues**.
16. **Server Load Management & Preventing DOS Attacks** - Use a **Rate Limiter**.
17. **Microservices Architecture** - Use an **API Gateway**.
18. **Single Point of Failure** - Implement **Redundancy**.
19. **Fault-Tolerance and Durability** - Implement **Data Replication**.
20. **User-to-User fast communication** - Use **Websockets**.
21. **Failure Detection in Distributed Systems** - Implement a **Heartbeat**.
22. **Data Integrity** - Use a **Checksum Algorithm**.
23. **Efficient Server Scaling** - Implement **Consistent Hashing**.
24. **Decentralized Data Transfer** - Consider using the **Gossip Protocol**.
25. **Location-Based Functionality** - Use **Quadtree** or **Geohash**.
26. **Avoid specific technology names** - Use **generic terms**.
27. **High Availability and Consistency Trade-Off** - Use **Eventual Consistency**.
28. **IP resolution & domain name query** - Mention **DNS**.
29. **Handling large data in network requests** - Implement **Pagination**.
30. **Cache Eviction Policy** - Prefer **LRU (Least Recently Used)** Cache.
31. **Handling traffic spikes** - Implement **Autoscaling** to manage resources dynamically.
32. **Analytics and audit trails** - Consider using **data lakes** or **append-only databases**.
33. **Handling large-scale simultaneous connections** - Use **Connection Pooling** and consider using **Protobuf** to minimize data payloads.

**Credit**: Dinesh Varyani


# What do Amazon, Netflix, and Uber have in common?  

They are extremely good at **scaling their system** whenever needed.  

Here are **8 must-know strategies** to scale your system:  

### 1 - Stateless Services  
Design stateless services because they don’t rely on server-specific data, making them easier to scale.  

### 2 - Horizontal Scaling  
Add more servers to **distribute the workload** across multiple instances.  

### 3 - Load Balancing  
Use a **load balancer** to distribute incoming requests evenly across multiple servers.  

### 4 - Auto Scaling  
Implement **auto-scaling policies** to dynamically adjust resources based on real-time traffic.  

### 5 - Caching  
Use **caching** to reduce the load on the database and efficiently handle repetitive requests.  

### 6 - Database Replication  
Replicate data across multiple nodes to **scale read operations** and improve redundancy.  

### 7 - Database Sharding  
Distribute data across multiple instances to **scale both write and read operations**.  

### 8 - Async Processing  
Move time-consuming and resource-intensive tasks to **background workers** using async processing to scale out new requests.  

---

**Over to you:** Which other strategies have you used?  

