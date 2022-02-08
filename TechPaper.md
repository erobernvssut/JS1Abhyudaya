
# Scaling

**Description**

You joined a new project. The project is going through some performance and scaling issues. After some analysis, the team lead asks you to investigate the possibility of using load balancers and understand vertical/horizontal scaling solutions.



## 1. Importance of Scalability

Scalability is a critical feature of corporate software. Prioritizing it from the beginning results in lower maintenance costs, a great user experience, and increased agility. The lifetime worth of software is determined by its quality, and creating with high scalability preserves both time and money over the long term.

## 2. User Case
- **Single-player desktop games:**
Each gamer downloads the game to their computer and they no longer need to be connected to the server. Your single-player game will stay single-player regardless of how many people are participating. No server will ever be overburdened. You, on the other hand, do not have a server that can be brought down by millions of users.

- **Social-media App:**
It is an app that requires a central server and connects to the network, it's clear that scalability is a concern. Because of the network connections, this software can only be used by a limited number of people. As a result, the more users that use this system at the same time, the more likely it is that the application may crash due to overload.

## 3. Constraints of Scalability
- **Synchronous Communication:**
It is a sort of communication between nodes or resources. In this case, whenever one node requests anything from another node, it will "block" (that is, it will wait and do nothing else) until it receives a response back.

- **Centralization:**
What would happen if our single-server i.e, a centralized system suddenly received an influx of request; 
Let’s say that our single-server system can probably process 100 requests per second; if it suddenly began receiving 10,000 requests a second, there is only so much that it can really do. No matter what our setup, with enough requests, we’ll run into the computational limitation of our centralized system.
The same could be said of handling requests; if our system had to deal with an influx of data to process.

## 4. Load Balancers
Scaling a load balancer lets you adjust its performance to its workload by changing the number of nodes the load balancer contains. You can scale load balancers up or down at anytime to meet your traffic needs. You can scale a load balancer to adjust its performance to its workload. 

In this model, there is a dispatcher that determines which worker instance will handle the request based on different policies. The application should best be "stateless" so any worker instance can handle the request






![Load Balancer](http://1.bp.blogspot.com/_j6mB7TMmJJY/TLnj_mWL50I/AAAAAAAAAgg/JFPsfGcAenI/s1600/p1.png)


## 5. Vertical Scaling
Vertical scaling or scaling up is the process of upgrading or adding resources to the existing system infrastructure on demand. Vertical scaling is based on the idea of adding more power(CPU, RAM) to existing systems, basically adding more resources.
Vertical scaling is not only easy but also cheaper than Horizontal Scaling. It also requires less time to be fixed.
![VS](https://middleware.io/wp-content/uploads/2021/09/What-is-Vertical-Scaling.png)

## 6. Horizontal Scaling
Horizontal scaling or scaling out refers to integrating additional server nodes or machines into your existing system infrastructure. Nonetheless, horizontal scalability may make the software architecture too complex, hence such a solution may require special expenses on maintaining its work It is horizontal scaling that is most often used to create software with the possibility of further growth for more users. Horizontal scaling is based on the idea of adding more machines into our pool of resources.
![HS](https://middleware.io/wp-content/uploads/2021/09/What-is-Horizontal-Scaling.png)

## 7. Analysing which is to be preffered
- **Cost** - Initial hardware costs for horizontal upgrades are higher. If you are working on a tight budget and need to add more resources to your infrastructure quickly and cheaply, then vertical scaling may be the best option for you.
- **Topographic distribution** - If you plan to have nationwide or global clients, it is unreasonable to expect them all to access your services from a single machine in a single location. In a situation like this, you’ll need to horizontally scale your resources.
- **Performance** -Horizontal scaling or scaling out allows you to combine the computing power of multiple servers and machines into one resource pool. This will no doubt offer a significant and drastic improvement in performance as well as the capacity of your application to handle more requests.
- **Reliability** - Horizontal scaling may offer you a more reliable system. It increases redundancy and ensures that you are not relying on a single machine. If one machine fails, another may be able to pick up the slack temporarily.


## References

 - [Cloudzero.com](https://www.cloudzero.com/blog/horizontal-vs-vertical-scaling)
 - [Middleware.io](https://middleware.io/blog/vertical-vs-horizontal-scaling/)
 
