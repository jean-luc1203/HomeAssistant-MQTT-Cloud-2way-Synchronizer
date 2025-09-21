## HAOS Encrypted MQTT Cloud Topic Synchronizer

**Description**

This HAOS add-on module establishes a secure TLS connection to a cloud MQTT broker. 
It enables transparent bidirectional synchronization between HAOS and external MQTT clients.
The MQTT client freely creates topics and their content on the broker.

These topics are automatically recreated as dynamic entities in HAOS, with real-time updates of values. 
Conversely, HAOS entities are published to the broker securely. 

**No additional local infrastructure (VPN, proxy, dynamic DNS) is required**, only Internet access is sufficient. 
Local security and data transit security are guaranteed by the **TLS** server certificate.

**Example of use**

An ESP32 connected to 4G in a second home can send its data to Home Assistant via this secure MQTT cloud broker.

The MQTT client creates and publishes its topics with formatted data, which are automatically recognized and reproduced as dynamic entities in HAOS. 

There is no need to manually create entities or plan the data received in advance. 

The user can simply organize these entities into custom dashboards for real-time visualization.
