## 1.0.0

## ⚡️ Module creation

This HAOS add-on module establishes a secure TLS connection to a cloud MQTT broker. 
It enables transparent bidirectional synchronization between HAOS and external MQTT clients. 

The MQTT client freely creates topics and their content on the broker.

These topics are automatically recreated as dynamic entities in HAOS, with real-time updates of values. 
Conversely, HAOS entities are published to the broker securely.

No additional local infrastructure (VPN, proxy, dynamic DNS) is required, only Internet access is sufficient. Local security and data transit security are guaranteed by the TLS server certificate.