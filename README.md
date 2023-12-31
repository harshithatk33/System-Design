# System-Design

System Design questions and solutions

Components of System Design
Below are some of the major components of the System Design. discussed in brief. The detailed version of this will be discussed in different posts:

## Load balancers:

Most crucial component for scalability, availability, and performance measures for systems.

## Key Value Stores:

It is a storage system similar to hashtables where key-value stores are distributed hash tables.

## Blob Storage:

Blob stands for binary large objects, as the name suggests is storage for unstructured data such as YouTube, and Netflix.

## Databases:

It is an organized collection of data so that they can be easily accessed and modified.

## Rate Limiters:

These sets the maximum number of requests a service can fulfill.

## Monitoring System:

These are basically software where system administrator monitor infrastructures such as bandwidth, CPU, routers, switches, etc.

## Distributed System Messaging Queue:

Transaction medium between producers and consumers.

## Distributed Unique ID generator:

In the case of large distributed systems, every moment multiple tasks are occurring so in order to distinguish it assign a tag corresponding to every event.

## Distributed Search:

Over every website, crucial information that visitors will seek is put into the search bar.

## Distributed Logging Services:

Tracing sequences of events from end to end.

## Distributed Task Scheduler:

Computational resources such as CPU, memory, storage, etc.

## System Design Priciples

System Design mostly follows the following principles

-   CAP (Consistency, Availability, Partition Tolerance)
-   BASE (Basically Available, Soft State, Eventual Consistency)
-   SOLID
-   KISS (Keep It Simple, Stupid!)

### CAP (Consistency, Availability, Partition Tolerance)

CAP theorem states that any distributed data store can only provide two of the following three guarantees:

1. Consistency - Every read receives the most recent write or an error.
2. Availability - Every request receives a response.
3. Partition tolerance - The system continues to operate in network faults.

### BASE (Basically Available, Soft State, Eventual Consistency)

The ACID (Atomicity-Consistency-Isolation-Durability) model used in relational databases is too strict for NoSQL databases. The BASE principle offers more flexibility, choosing availability over consistency. It states that the states will eventually be consistent.

### SOLID

SOLID principle is quite famous in OOP. There are 5 components to it.

1. SRP (Single Responsibility Principle)
2. OCP (Open Close Principle)
3. LSP (Liskov Substitution Principle)
4. ISP (Interface Segregation Principle)
5. DIP (Dependency Inversion Principle)

## KISS (Keep It Simple, Stupid!)

"Keep it simple, stupid!" is a design principle first noted by the U.S. Navy in 1960. It states that most systems work best if they are kept simple.
