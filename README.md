# OTelCollectorDemo
This project is a demo of hooking up a Spring Boot Microservice to Grafana Loki, Tempo and Mimir, according to OpenTelemetry Protocol.

A Spring Boot Microservice serves HTTP requests, and is configured with the OpenTelemetry SDK to send logs, metrics and traces to a remote collector. The Microservice is hosted on a remote linux server. 

The two configurations I am exploring are the collector configuration and the agentic configuration. This project is the collector configuration. 

Under the collector configuration, there are two options to choose from:
1. Sending to a local collector, then querying that collector from a remote machine by connecting it to an observability backend on a remote machine (or Grafana cloud)
2. Sending it to a remote collector, then sending it to an observability backend located on the same machine as the collector.

(Corrections to be made as the purpose of this project is to further my understanding of setting up observability using the OpenTelemetry protocol)
