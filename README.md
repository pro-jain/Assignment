# Internship Learning & Implementation Report


# Topics Covered

## 1. Field Oriented Control (FOC)

Studied the fundamentals of Field Oriented Control (FOC) used in motor control applications.

---

## 2. Apache Kafka

Learned the architecture and working of Apache Kafka as a distributed event-streaming platform.

### Concepts Covered

- Kafka Architecture
- Producers
- Consumers
- Brokers
- Topics
- Partitions

### Implementation

Implemented producer and consumer applications to understand asynchronous event streaming and message handling.

Implementation Repo: https://github.com/abhaynextflyt/utilities/tree/bodhini

---

## 3. RabbitMQ (Message Broker)

Studied RabbitMQ for asynchronous communication between applications.

### Concepts Covered

- Message Queues
- Exchanges
- Queues
- Producers and Consumers
- Direct Exchange
- Fanout Exchange
- Topic Exchange

---

## 4. Redis

Learned Redis as an in-memory data store used for high-speed data access and communication.

### Topics Covered

- Key-Value Storage
- Strings
- Publish/Subscribe (Pub/Sub)
- Caching
- Fast Data Retrieval

---

## 5. Proxy Server & Load Balancing

Implemented a basic HTTP Proxy Server using Node.js and studied different load balancing strategies used in distributed systems.

### Concepts Learned

- Client-Server Architecture
- Request Forwarding
- Response Forwarding
- HTTP Methods
- Proxy Workflow
- Reverse Proxy
- Round Robin Load Balancing
- Least Connections Algorithm

---

# Implementation

## Distributed Camera Streaming System using Proxy Server and Redis

Designed and implemented a distributed camera streaming system consisting of multiple camera sources, multiple frontend clients, multiple backend processing servers, a proxy server, and Redis for maintaining backend server capacity information.

### Workflow

1. Multiple cameras continuously capture video streams.
2. Frontend clients send requests to the Proxy Server for a camera feed.
3. The Proxy Server queries Redis to determine the current load and capacity of all backend servers.
4. Based on the available capacity, the Proxy Server selects the most appropriate backend server.
5. The selected backend server receives and processes the requested camera stream.
6. The processed stream is returned to the Proxy Server.
7. The Proxy Server forwards the processed stream to the requesting frontend client.
8. Redis is continuously updated with backend server capacity information, enabling efficient load balancing for future requests.

### Implementation Repo: https://github.com/abhaynextflyt/reccesys001/tree/bodhini/redis-camera-streams

---

