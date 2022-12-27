# Walking through optimization in GKE

In this repository, we'll be using the `microservices-demo` repository to deploy a multi-tier web application to GKE. 

Using this application, we will walk through GKE functionality that enables users to optimize their cost and performance.

## Overview

We can think of optimization in GKE around a handful of related areas:

* Culture
* Cluster bin packing
* App right-sizing
* Demand based downscaling

Optimizing Kubernetes requires performing tasks across these areas. These tasks include:

* Understanding cluster usage
* Understanding app usage
* Adjusting app requests and limits
* Adjusting autoscaling configuration

These tasks are not one-offs; rather they are part of a continuous effort to optimize as workloads onboard, offboard, and change according to demand and usage. 

## Setup

We can start by cloning the repository for the `microservices-demo`. 

```
git clone https://github.com/GoogleCloudPlatform/microservices-demo.git
cd microservices-demo
```

We will then perform steps 1 - 5 in the `README.md`. This will ensure we have a GCP project, a GKE cluster, and the microservices that make up the web application running in that cluster.