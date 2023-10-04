---
layout: post
author: vipul
title: Loadbalancer
summary: Load balancing is a key component of highly-available infrastructures commonly used to improve the performance and reliability of web sites, applications, databases and other services by distributing the workload across multiple servers.
date: 2023-10-04 1:36:23 +0530
category: ['loadbalancer']
keywords: loadbalancer function, loadbalancer case study, summary  
tags: Loadbalancer
thumbnail: /assets/img/posts/loadbalancer.png
usemathjax: true
permalink: /blog/loadbalancer/
---

if many users try to access the server simultaneously and it is unable to handle the load, they may experience slow load times or may be unable to connect at all.
![loadbalancer](/assets/img/posts/img.png)

This single point of failure can be mitigated by introducing a load balancer and at least one additional web server on the backend.

![loadbalancer](/assets/img/posts/Diagram_1.png)
What kind of traffic can load balancers handle?

- **HTTP :** Standard HTTP balancing directs requests based on standard HTTP mechanisms. The Load Balancer sets the X-Forwarded-For, X-Forwarded-Proto, and X-Forwarded-Port headers to give the backends information about the original request.
- **HTTPS**: HTTPS balancing functions the same as HTTP balancing, with the addition of encyption. Encryption is handled in one of two ways.
  - Either with SSL Passthrough which maintains encryption all the way to the backend
  - or SSL termination which places the decryption burden on the load balancer but sends the traffic unencrypted to the back end.
- **TCP:**  For applications that do not use HTTP or HTTPS, TCP traffic can also be balanced. for example, traffic to a database cluster could be spread across all of the servers.
- **********UDP:********** More recently, some load balancers have added support for load balancing core internet protocols like DNS and syslogd that use UDP.

Load Balancing Algorithms

**Source:**  hash of the source IP of the request, such as the visitor’s IP address. same user connects to the same server.

![loadbalancer alogrithms](/assets/img/posts/loadbalnceralgorithms.jpg)

## Redundant Load Balancer

to remove the load balancer as a single point of failure, a second load balancer can be connected to the first to form a cluster, where each one monitors the other’s health. Each one is equally capable of failure detection and recovery.

![loadbalancer](/assets/img/posts/Diagram_2.png)

In the event the main load balancer fails, DNS must take users to the second load balancer. Because DNS changes can take a considerable amount of time to be propagated on the Internet and to make this failover automatic, many administrators will use systems that allow for flexible IP address remapping, such as Reserved IPs.

On Demand IP address remapping eliminates the propagation and caching issues inherent in DNS changes by providing a static IP address that can be easily remapped when needed. the domain name can remain associated with the same IP address, while the IP address itself is moved between server.

![loadbalancer](/assets/img/posts/ha-diagram-animated.gif)