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
