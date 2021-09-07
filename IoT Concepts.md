# IoT Concepts
 Topics and concepts that should be included in the 420-6P3 Connected Objects course
 
 ## Device Management & Provisioning
 
### Microchip “Provisioning” vs. Microsoft “Provisioning”
See example from [this repo](https://github.com/Azure-Samples/Microchip-PIC-IoT-Wx)

![diagram of microchip provisioning with local PC tool](https://github.com/Azure-Samples/Microchip-PIC-IoT-Wx/raw/main/media/image4.png)
 
 ### Provisioning Examples
 
 #### Azure's Device Provisioning Service (DPS)
 Device Provisioning Service (DPS): a helper service for IoT Hub that enables zero-touch, just-in-time provisioning to the right IoT hub without requiring human intervention, allowing customers to provision millions of devices in a secure and scalable manner
 
 ### Management at Scale
 
 How to setup automatic device management at scale
 
 Must be able to filter and query data in order to select specific devices.
 
 ### Getting Connection state
 
 **Heartbeat patter**
 Device sends a small message at small intervals. Setup a watcher to trigger if the device has been silent for too long.
 
 **Device disconnected event**
 Setup an event watcher to fire on a device disconnected event
 
 **Monitor and Resource Health service**
 Some cloud service providers offer the service of specifically monitoring device health. For example, Azure Monitor and Resource Health feature. 
 
 ## Device Twins/Shadows
 
 Set, get and syncronize the state of a device from a JSON object that is hosted in the cloud.
 Called device twin in Azure and device shadow in AWS.
 
 See [Azure Device Twins](IoT%20Cloud%20Service%20Providers.md#Device%20Twins) for more.
 
 ## Security
 
 ### Certificates

 - Types of certificates
	 - Symmetric
	 - X.509
 - Creating and adding client certificates to devices
	 - Certificate signing
 - Certificate vulnerabilities
	 - leakage
	 - JTAG sniffing

#### Resources & Guides
 [AWS IoT EduKit is what? What can we learn from it?](https://ma2shita.medium.com/aws-iot-edukit-is-what-what-can-we-learn-from-it-96039238d712) by Kohei Matsushita
 
 ## IoT Communication Protocols
 
 ### MQTT
 
 Video [compares MQTT to HTTP](https://youtu.be/ybuSYCqRWYM?t=491)
 
 ## Message Routing
 
 Routing messages between devices, pub/sub servers and other back-end services such as storage, filtering and alerting.
 
 