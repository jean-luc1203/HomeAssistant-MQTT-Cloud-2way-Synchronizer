## HAOS Encrypted MQTT Cloud Topic Synchronizer

**<u>Description:</u>**

This HAOS add-on module establishes a secure TLS connection to a cloud MQTT broker. 
It enables transparent bidirectional synchronization between HAOS and external MQTT clients.
The MQTT client freely creates topics and their content on the broker.

These topics are automatically recreated as dynamic entities in HAOS, with real-time updates of values. 
Conversely, HAOS entities are published to the broker securely. 

**No additional local infrastructure (VPN, proxy, dynamic DNS) is required**, only Internet access is sufficient. 
Local security and data transit security are guaranteed by the **TLS** server certificate.

<u>Example of use:</u>

An ESP32 connected to 4G in a second home can send its data to Home Assistant via this secure MQTT cloud broker.

The MQTT client creates and publishes its topics with formatted data, which are automatically recognized and reproduced as dynamic entities in HAOS. 

There is no need to manually create entities or plan the data received in advance. 

The user can simply organize these entities into custom dashboards for real-time visualization.

<u>Topic example:</u>

* One config topic for the autodiscovery HA
* One state topic for the relatime value
  
Below, what you can see once you are connected to the Cloud Broker (in my case, HiveMQ):

<img width="597" height="259" alt="image" src="https://github.com/user-attachments/assets/587d1472-ac84-4f31-bf16-4e9fafa251a7" />

Here is what this will automatically create in Home Assistant.
The data is refreshed as soon as it is modified by the source (i.e., the MQTT client).

<img width="986" height="337" alt="image" src="https://github.com/user-attachments/assets/70c4b1de-0665-468a-b6aa-b44468bff202" />


