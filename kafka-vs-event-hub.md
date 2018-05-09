|   | Confluent Open Source   | HDInsight Kafka | Azure Event Hub |
|:------------- |:---------------|:-------------|:-------------|
|              |         |            |               |
| Support by open source componentes | good | good      |            restricted |
| Support by StreamSets Data Collector | yes | yes      |            yes |
| Support by Spark Structured Streaming | yes | yes       |            no |
| Support by Kafka Streams | yes | yes       |  no (only via Kafka Connect bridge to Kafka) |
| Support by Azure Stream Analytics | yes | yes       |  yes |
| Supports REST | yes (with REST proxy)  | (with REST proxy) | yes |
| Supports AMQP | no  | no | yes |
| Supports MQTT | no  | no | no |
| Supported Clients       | Java, .Net, Go, Phyton, C++ | | .Net, Java |
| Supports Avro       | yes| yes | no |
| Surrounding components       | Kafka Connect, Kafka Streams, | yes | Event Hubs Capture, Azure Event Grid, Azure Stream Analytics, Azure Functions|
|              |         |            |               |
| Available on-premises | yes        | no |           no |
| Available as a service | no        | yes |       yes |
| Cross-region replication | yes | yes | yes | 
| Multi-region replication | yes (with MirrorMaker or Confluent Replicator) | yes (with MirrorMaker or Confluent Replicator) | no | 
| Throttling | yes (through Quotas) | yes (through Quotas) | yes | 
| Maximum message size | no limit (default 1MB) | no limit (default 1MB) | limit on 256K for basic or standard sized Event Hub, 1MB for [dedicated](https://azure.microsoft.com/de-de/blog/event-hubs-dedicated-offering/) | 
| Authentication | optional (SASL, kerberos) | optional (kerberos, Ranger) | mandatory (SAS based) |
| Authorization | optional (ACL) | optional (ACL, Ranger) | ? |
| Monitoring | Kafka Manager, Confluent Control Center (commercial) | through Ambari |  |
| Replayability | yes | yes | yes |
| Data Retention | no limit (never, time- & size-based, key-based) | no limit  (never, time- & size-based, key-based) | 1|
| Scalability | yes | yes | yes |
| In-order delivery | yes (per partition) | yes (per-partition) | yes (per-partition) |

 
