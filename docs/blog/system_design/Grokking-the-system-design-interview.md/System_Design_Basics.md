# System Design Basics

## Key Characteristics of Distributed Systems

### Scalability

**Definition**: The capability to grow and manage increased demand, such as increased data volume, number of transactions.

* Horizontal scaling:  [Cassandra](https://en.wikipedia.org/wiki/Apache_Cassandra) and [MongoDB](https://en.wikipedia.org/wiki/MongoDB)
* Vertical scaling: e.g. MySQL

### Reliability

**Definition**: The probability a system will fail in a given period.



### Availability

**Definition**: The time a system remains operational to perform its required function in a specific period.



### Efficiency

Definition:

The response time(latency) means the delay to obtain the first item.

The throughput(bandwidth) number of items delivered in a given time unit (e.g., a second)

### Manageability or Serviceability.

How easy it is to operate and maintain.

## Load Balancing(LB)

Between the user and the web server

Between web servers and an internal platform layer, like application servers or cache servers

Between internal platform layers and database.

### Redundant Load Balancers

## Caching

recently requested data is likely to be requested again

* Application server cache
* Content Delivery Network(CDN) for static media.
* Cache Invalidation
  * **Write-through **
  * **Write-around**
  * **Write-back**
* Cache eviction
  * First In First Out (FIFO)
  * Last In First Out (LIFO)
  * Least Recently Used (LRU)
  * Most Recently Used (MRU)
  * Least Frequently Used (LFU)
  * Random Replacement (RR)

## Data Partitioning

Definition: a technique to break a big database (DB) into many smaller parts

### Partition Methods

* Horizontal Partitioning. **(Data Sharding)** Different rows in different tables. Range-based partitioning. It may lead unbalanced servers.
* Vertical Partitioning. Store tables related to a specific feature in their own server.
* Directory-Based Partitioning: create a lookup service that knows your current partitioning scheme and abstracts it away from the DB access code

### Partitioning Criteria

* **Key or Hash-based Partitioning**: apply hash function to the entity's attribute, get partition number.
* List Partitioning: each partition has a list of values.
* **Round-robin partitioning**
* **Composite Partitioning**

### Common Problems of Data Partitioning

* **Joins and Denormalization**
* **Referential integrity**
* **Rebalancing**

## Indexes

