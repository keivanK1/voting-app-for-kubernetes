# voting-app-for-kubernetes

This repository contains voting app pods and services for testing.

## Requirements

Google cloud account with activated kubernetes cluster and nodes.

## Getting started

* clone the project
* create voting app pod:

        kubectl create -f voting-app-pod.yml
* create service of voting app:

        kubectl create -f voting-app-service.yml
* create redis pod:

        kubectl create -f redis-pod.yml
* create service of redis:

        kubectl create -f redis-service.yml
* create postgres database pod:

        kubectl create -f postgres-pod.yml
* create service of postgres database:

        kubectl create -f postgres-service.yml
  * this service will enable the other component to access postgres database.
* create worker pod:

        kubectl create -f worker-app-pod.yml
* create result pod:

        kubectl create -f result-app-pod.yml
* create result service:

        kubectl create -f result-service.yml