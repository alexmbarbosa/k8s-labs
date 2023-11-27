# K8s Kafka Playground

This project aims to set up a Kafka development environment on Kubernetes.
Initially, it includes configurations for:

* Namespace(s)
* Zookeeper
* Kafka broker(s)

## Project Structure

The project consists of the following components:

### Namespace Manifest

The `kafka-lab-namespace.yaml` file defines the Kubernetes namespace for isolating the Kafka components and their resources.

### Zookeeper

Zookeeper plays a crucial role in coordinating the distributed systems in Kafka. The setup for Zookeeper is included in the project to support Kafka's functionality.

### Kafka Brokers

The project includes configurations and setups for Kafka brokers. These brokers are responsible for handling message storage and processing within the Kafka environment.

## How to Use

To deploy this Kafka lab in your Kubernetes environment, follow these steps:

1. **Namespace Deployment:**
   Apply the `kafka-lab-namespace.yaml` manifest to create a dedicated namespace for Kafka components.

2. **Zookeeper Deployment:**
   Deploy the Zookeeper using the provided configurations. Ensure Zookeeper is running and accessible.

3. **Kafka Broker Deployment:**
   Configure and deploy the Kafka brokers within the Kubernetes environment to establish the messaging system.

4. **Testing:**
   Test the functionality of the Kafka setup by producing and consuming messages through Kafka topics.

## Prerequisites

- Docker
- Kubernetes engine (k3s, kind, minikube, etc)
- kubectl installed
- Basic understanding of Kafka and Kubernetes concepts
