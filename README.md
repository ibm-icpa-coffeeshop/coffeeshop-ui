# coffeeshop-service
Appsody version of the coffeeshop BFF service, part of the reactive coffeeshop demo.

To deploy:
1. Ensure have kafka running in your Kubernetes cluster.
2. Update appsody-deploy.yaml to confgiure the Kafka bootstrap server host and port:

```yanl
env:
  - name: MP_MESSAGING_CONNECTOR_LIBERTY_KAFKA_BOOTSTRAP_SERVERS
    value: my-cluster-kafka-bootstrap.kafka.svc:9092
```