---
layout: post
published: true
title: 	AWS Well Architected Framework

---
Architectural best practices should be followed to reduce interdependencies between systems.

**Asynchronous integration** - this is another form of loose coupling where an interaction does not need an immediate response (think SQS queue or Kinesis)

**Graceful failure** - build applications such that they handle failure in a graceful manner (reduce the impact of failure and implement retries). Auto Scaling helps to reduce the impact of failure by launching replacement instances

**Well-defined interfaces** - reduce interdependencies in a system by enabling interaction only through specific, technology-agnostic interfaces (e.g. RESTful APIs). A relational database is not an example of a well-defined interface

**Service discovery** - disparate resources must have a way of discovering each other without prior knowledge of the network topology. Usually DNS names and a method of resolution are preferred over static IP addresses which need to be hardcoded somewhere
Though automatic scaling for storage and database provides scalability (not necessarily elasticity), it does not reduce interdependencies between systems

