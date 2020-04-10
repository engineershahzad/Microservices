# Microservices 

In 1972, David Parnas  introduced concept of Modularization  on the 
principle of decomposing a large, complex software system into “Loosely 
coupled, highly cohesive”

Microservices Architecure  is a software development technique  which arranges an application as a collection of loosely coupled,  highly cohesive services.
 The term, “loosely coupled” means the dependency between modules should be very low and “highly cohesive” means that one module should focus on single or similar functionality.

It  is an approach to developing a single application as a suite of small services, each running in its own process and communicating with lightweight mechanisms,  often an HTTP resource API.

In February 2020, the Cloud Microservices Market Research Report predicted that the global microservice architecture market size
 will increase at a CAGR of 21.37% from 2019 to 2026 and reach  $3.1 billion by 2026.

# Monolithic vs. Microservices Architecture: An Introduction

A  monolithic architecture  is a unified model for designing a software solution. All components of software here are interconnected and interdependent.
Monolithic software only supports one programming language, it is not possible to implement one single module of it in other programming language.

In such a tightly coupled architecture, each component and its related components must be functional in order for the code to be executed or compiled successfully.

Microservices architecture  on the other hand, is a modular approach for designing a software solution.
Herein, a software application is built with an independent group of components that run each application process as a service.
 
In such a loosely coupled architecture, a component is independent of the other one, can be written in different programming languages,  use different data storages, and serves only one specific function.


# Monolithic vs. Microservices Architecture: Differences

## Fault Isolation

Since all services in a microservice architecture are independent of each other, any halt in a process will keep the rest of the processes unaffected.	

For example, a memory leak in one service will only affect that single service. A change to a small part of the application only requires rebuilding and redeploying only one or a small number of services.

On the other hand, any misbehaving component in a monolithic architecture will bring the entire application down (since all services are interconnected and interdependent).

For example, In the monolithic approach, an application supporting three functions would have to be scaled in its entirety even if only one of these functions had a resource constraint.

With microservices, only the microservice supporting the function with resource constraints needs to be scaled out, thus providing resource and cost optimization benefits.


# Benefits

## Technology Commitment

With a microservices architecture, developers have the advantage of using different technologies (languages, frameworks, and OS) to build an application.
This eliminates dependency and long-term commitment with a single technology stack.

Whenever a new service is built or an existing service is updated, a new, better technology stack can be adopted.					     
This also eliminates the dependency of the development team on a particular resource for building or updating a service

In a monolithic architecture, the development team is forced to stick to a single technology, which has its own limitations.
For example, if a framework that your application uses become obsolete with time, migrating to a newer, better framework can be challenging.

The development team may have to rewrite the entire application in a new language or on a different framework, which involves risks			 and is time-consuming as well.  

## Modularity

This makes the application easier to understand, develop, test, and become more resilient to architecture erosion.				     This benefit is often argued in comparison to the complexity of monolithic architectures.
## Scalability

Since microservices are implemented and deployed independently of each other, i.e. they run within independent processes,they can be monitored and scaled independently.

Since the services are independent of each other, continuous deployment of new features and application scaling can be done with ease.
If a service goes down, it won’t affect the functionality of the entire application

## Integration of differnt and legacy systems:

Microservices is considered as a viable mean for modernizing existing monolithic software application.

There are experience reports of several companies who have successfully replaced  their existing software by microservices, or are in the process of doing so using  an incremental approach.

## Distributed development:

It parallelizes development by enabling small autonomous teams to develop, deploy and scale their respective services independently.

Microservice-based architectures facilitate continuous integration, continuous delivery and deployment.
 

## Criticism and Concerns

Inter-service calls over a network have a higher cost in terms of network latency and message processing time than in-process calls within a monolithic service process.

Development and support of many services is more challenging if they are built with different tools and technologies. This is especially a problem if engineers move between projects frequently.

The protocol typically used with microservices (HTTP) was designed for public-facing services, and as such is unsuitable for working internal microservices that often must be reliable.

While not specific to microservices, the decomposition methodology often uses functional decomposition, which does not handle changes in the requirements while still adds the complexity of services.

The very concept of microservice is misleading, since there are only services. There is no sound definition of when a service starts or stops being a microservice.
