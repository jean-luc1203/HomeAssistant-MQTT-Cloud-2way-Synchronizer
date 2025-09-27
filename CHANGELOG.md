## 1.0.2

## 🐞 Bug resolution

Changed permissions on scripts


## 1.0.1

## 🐞 Bug resolution

Add URL for HAOS dynamic API. Allows use of an HTTPS connection.
The JSON file for entities is copied correctly if it does not exist.
The publication topic is set to mqtt-cloud-synchronizer/.
Miscellaneous. 

## 👀 To do

It remains to be tested whether the file contains entities that do not exist. Handle the absence and do not have an error message in the log.


## 1.0.0

## ⚡️ Module creation

This HAOS add-on module establishes a secure TLS connection to a cloud MQTT broker. 
It enables transparent bidirectional synchronization between HAOS and external MQTT clients. 

The MQTT client freely creates topics and their content on the broker.

These topics are automatically recreated as dynamic entities in HAOS, with real-time updates of values. 
Conversely, HAOS entities are published to the broker securely.

No additional local infrastructure (VPN, proxy, dynamic DNS) is required, only Internet access is sufficient. Local security and data transit security are guaranteed by the TLS server certificate.