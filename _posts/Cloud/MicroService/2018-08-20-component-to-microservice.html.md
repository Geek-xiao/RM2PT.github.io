---
layout: post
title: MicroServices
date: 2018-08-20 06:23:00.000000000 +08:00
categories: [Cloud, MicroService]
author: yyl
---

## MicroServices

**MircoService** = `Component` + `Standard Interface` (RESTFul with JSON) + `Supported Environment` (Authentication / Health Check / Metrics / Tracing / Fault Tolerance / Standard API Document)

### Java EE MicroServices (MicroProfile)

`MicroProfile` specifies a collection of Java EE APIs and technologies which together form a core baseline microservice that aims to deliver application portability across multiple runtimes.

Eclipse MicroProfile = `CDI` + `JAX-RS` + `JSON-P/JSON-B` + `MPs` (MP config / MP Fault Tolerance / MP Health Check / JWT Authentication / MP Metrics/ OpenAPI / OpenTracing / Rest Client)

#### * Fault Tolerance

**Eclipse MicroProfile Fault Tolerance** provides the ability to separate execution logic from business logic. Key aspects of the API include TimeOut, RetryPolicy, Fallback, Bulkhead, and Circuit Breaker processing.

#### * Health Check

**Eclipse MicroProfile Health Check** provides the ability to probe the state of a computing node from another machine

#### * JWT Authentication

**JWT** Authentication provides role based access control (RBAC) microservice endpoints using OpenID Connect (OIDC) and JSON Web Tokens (JWT).

#### * Metrics

**MicroProfile Metrics** provides a unified way for MicroProfile servers to export monitoring data to management agents. Metrics will also provide a common Java API for exposing their telemetry data.

#### * OpenAPI

**OpenAPI** provides a unified Java API for the [`OpenAPI v3 specification`](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.0.md) that all application developers can use to expose their API documentation

#### * OpenTracing

**MicroProfile OpenTracing** defines an API and associated behaviors that allow services to easily participate in a distributed tracing environment.

#### * MicroProfile Rest Client

**Eclipse MicroProfile Rest Client** provides a type-safe approach for invoking RESTful services over HTTP. The MicroProfile Rest Client builds upon the JAX-RS 2.1 APIs for consistency and ease-of-use.

### MicroProfile Implementations:

* Open Liberty (IBM WebSphere)
* WildFly Swarm (RedHat JBoss)
* Payara Mico (Glassfish)
* KumuluzEE
* Hammock
* Apache TomEE (Tomcat)

## Reactive MicroServices

Reactive Systems are Responsive, Resilient, Elastic and Message Driven.

* `Responsive`: The system responds in a timely manner if at all possible.

* `Resilient`: The system stays responsive in the face of failure.

* `Elastic`: The system stays responsive under varying workload.

* `Message Driven`: Reactive Systems rely on asynchronous message-passing to establish a boundary between components that ensures loose coupling, isolation and location transparency.

`Akka` and `Vert.x` are two commonly used reactive frameworks that run on top of the JDK

* `Akka` has indepented event queue.
* `Vert.x` uses Event Bus

## References

MicroService

* [Java EE 8 MicroService](https://www.udemy.com/java-ee-8-microservices/)
* [Eclipse MircoProfile](https://projects.eclipse.org/projects/technology.microprofile)
* [Eclipse MircoProfile](http://microprofile.io)
* [Delivering Microservices for Enterprise with DevOps](https://developer.capitalone.com/blog-post/delivering-microservices-for-enterprise-with-devops/)
* [Comparing and Contrasting Open Source BPM Projects](https://medium.com/capital-one-developers/comparing-and-contrasting-open-source-bpm-projects-196833f23391)
* [MicroProfile: 5 Things You Need to Know](https://dzone.com/articles/microprofile-5-things-you-need-to-know)

Reactive MicroService

* [The Reactive Manifesto](https://www.reactivemanifesto.org)
* [Microservices — When to React Vs. Orchestrate](https://medium.com/capital-one-developers/microservices-when-to-react-vs-orchestrate-c6b18308a14c)
* [Building Microservices: A Reactive Framework Comparison](https://medium.com/capital-one-developers/building-microservices-a-reactive-framework-comparison-fb49d8f3c8f4)
* [ReactiveX](http://reactivex.io)
