## Microservices - Fundamentals

See course https://www.coursera.org/learn/intro-ibm-microservices/

A microservice is an engineering approach focused on decomposing applications into 
single-function modules with well-defined interfaces which are independently deployed 
and operated by small teams who own the entire lifecycle of the service. 

Microservices accelerate delivery by minimizing communication and coordination between people 
while reducing the scope and risk of change

See [Intro to Microservices](https://medium.com/omarelgabrys-blog/microservices-with-spring-boot-intro-to-microservices-part-1-c0d24cd422c3)

**Main keywords:**
- decomposing
- single-function
- well-defined interfaces
- independent
- small teams
- entire lifecycle
- minimizing communication
- reducing the scope of change

### Blue-Green Deployment

- [Blue-Green Deployment](https://martinfowler.com/bliki/BlueGreenDeployment.html)

### Microservice Communication

- [Communication in a microservice architecture](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/communication-in-microservice-architecture)

### API Gateway

- [Building Microservices: Using an API Gateway](https://www.nginx.com/blog/building-microservices-using-an-api-gateway/)

### The Service Registry

- [An Introduction to Microservices, Part 3: The Service Registry](https://auth0.com/blog/an-introduction-to-microservices-part-3-the-service-registry/)

### Challenges of Microservices

[Microservice prerequisites](https://martinfowler.com/bliki/MicroservicePrerequisites.html)

- How can I find a service that I need? 
    - What if a service moves? 
    Which instance do I use if there are multiple instances? 
- Is that service up and running? 
    - What do I do if it's not running? 
- How can I scale my services? 
    - How do I spread my load over multiple instances? 
- How can I introduce new versions of services without impacting existing users? 
- How can I test against failures? 
    - How does the failure of one service affect other instances of the same service? 
    - How does the failure of one service affect other related services? 
- How can I protect against a catastrophic failure?
    - How do I prevent the failure of one service taking everything down?

The more pieces running independently, the more the network becomes an issue with latency and disconnects.

In the microservices environment failures will happen, hardware errors are just one example. 
So fault tolerance is needed to recover and carry on. 
Given the independent services that interact, data placement and interfaces have to be carefully planned. 
Add to the possibility of failure that you could corrupt data. 
These are important considerations while designing and using microservices architecture.

### DevOps

- [Continuous Delivery: Anatomy of the Deployment Pipeline](http://www.informit.com/articles/article.aspx?p=1621865)
- [Continuous Delivery](https://martinfowler.com/books/continuousDelivery.html)

### Useful links

- [So You’re Thinking of Decomposing Your Monolith into Microservices](https://blog.codeship.com/so-youre-thinking-of-decomposing-your-monolith-into-microservices/#disqus_thread)
- [Microservices: Decomposing Applications for Deployability and Scalability](https://www.infoq.com/articles/microservices-intro/)
- [Want to develop great microservices? Reorganize your team](https://techbeacon.com/app-dev-testing/want-develop-great-microservices-reorganize-your-team)
- [IaaS, PaaS and SaaS – IBM Cloud service models](https://www.ibm.com/cloud/learn/iaas-paas-saas)
- [Circuit Breakers and Microservices Architecture](https://techblog.constantcontact.com/software-development/circuit-breakers-and-microservices/)
- [Want to develop great microservices? Reorganize your team](https://techbeacon.com/app-dev-testing/want-develop-great-microservices-reorganize-your-team)
- [Microservice prerequisites](https://martinfowler.com/bliki/MicroservicePrerequisites.html)

