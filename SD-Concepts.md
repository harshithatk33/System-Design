## System Design Concepts

-   Increasing the capacity of the RAM or upgrading the CPU as and when the number of requests to the server increases is called as `Vertical Scaling`. Although this seems simple and easy it is very limiting.

-   A better way would be to add a duplicate server which can handle the subset of the requests which are coming from the users. Essentially, you would be adding a new server which would be very similar to the old one. This is called as `Horizontal Scaling`.

-   Horizontal Scaling is better as we can infinatly increase the servers as an when required and they would also contirubute to Availability. When a server crashes, the requests would be re-routed to other server which are up.

-   This approach brings in its own set of problems as it is quite complicated. There is a chance that one of the servers would be overloaded with requests.

-   `Load Balancers` can be used to handle such situations and they are also called as reverse-proxy.

-   They use algorithms such as Round-Robin or Hashing to re-route the traffic to the servers such that each server gets an equal amount of load.

-   When the servers are located in different geographical locations, we can configure the Load Balancers to route the requests to the nearest location.

-   If you are using your servers to just provide static content such as html, css or even js file, then you can use something called as the `Content Delivery Networks` or CDN. CDNs will not be running anything, they would just be a replicate of your server and they can be placed any where in the world.

-   CDNs can be kept update in a pull or push basis.

-   They are also a form of `Caching`. Caching is all about duplicating certain files which can contribute to faster retrival by servers. Usually computers/server have a copy of frequently accessed files within them. CPUs also have L1/L2/L3 Caching.

-   Every computer on the internet is assigned a unique number called as the `Internet Protocol Address` or the widely known `IP Address`.

-   `TCP` or the `Transmission Control Protocol` is a set of rules which are present for reliable transfer of data packets over the internet.

-   `Domain Name Servers (DNS)` are used to map a partcular domain name to an IP Address which can be used to find the location of the server.

-   `Hypertext Transfer Protocol (HTTP)` is an application layer protocol as an improvement over TCP. This protocol has a request-response model with headers and data body with other meta data which will be transfered.

-   `REST` is one of the most popular API Paradigms/Patterns which everyone follows, similar to REST we have SOAP, graphQL, gRPC. They work with HTTP APIs making them stateless and consistent. A request-response should contain status codes which exactly describes the status/output of the request.

-   `GraphQL` was introduced by facebook in 2015. In REST APIs we usually send multilpe requests to the server to get data unlike in GraphQL. In GraphQL, we can send one request to get multiple data, it would be like a query which describe what data we would need.

-   By using GraphQL, we get exactly what we asked for and we do not run the risk of overfeatching data which we do not need.

-   `gRPC` was released by Google in 2016, was developed to improve on REST. This is used for server-to-server communication, but `gRPC Web` is also gaining quite a lot of users which can be used similar to REST APIs.

-   The performance boost comes from Protocol Buffers for gRPC as they use serialized data instead of JSON which is used by REST. One of the downside is that JSON is human readable but Protocol Buffers are not.

-   Another application layer protocol is `Web Sockets`. Websockets allow for bidirectional communication.

-   Data can be stored in `SQL`, this way it can be more efficient to read and write data when compared to using text files. There are two types of database storages, SQL and NoSQL.

-   Relational Database Management Systems usually follow `ACID(Atomicity, Consistency, Isolated, Durability)` properties.

-   NoSQL database are different from RDMS where they do not follow a specified schema and they usually follow the `BASE (Basically Available, Soft State, Eventual Concistancy)` properties.
