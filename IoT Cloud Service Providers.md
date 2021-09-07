# Cloud Service Providers
Beginner and Professional services for deploying, hosting, distributing or maintaining IoT systems.

## Azure

Students get 100$ of credit for 12 months (no renewals) and free developer tools without a credit card. See [details here](https://azure.microsoft.com/en-us/free/students/).

### Azure IoT Explorer
Stand alone software running locally that helps visualize and manage devices connected to Azure IoT Hub. See details in the [azure-iot-explorer github wiki](https://github.com/Azure/azure-iot-explorer/wiki).

### Azure IoT Hub

Central messaging hub for bi-directional communication between an IoT application and it's devices. Can managed secure connections between devices, routing and back-end services such as filtering, storage, monitoring, alerts, data visualization, etc.

For details and guides see [Azure IoT Hub Documentation](https://docs.microsoft.com/en-us/azure/iot-hub/)


### Tooling
- Azure Portal (web interface)
	- unpractical for large set of devices
- Azure CLI
- IoT Hub SDKs
- REST APIs

#### Azure CLI

Azure CLI is a "general" command line interface for managing Azure services. Some specific services such as Azure IoT Hub require the intallation of extensions.

##### Azure IoT CLI Extension (az iot)
The Azure IoT extension for Azure CLI aims to accelerate the development, management and automation of Azure IoT solutions.

See the [az iot extension repository here](https://github.com/Azure/azure-iot-cli-extension).

See official `az iot` reference on [Microsoft Docs](https://docs.microsoft.com/en-us/cli/azure/ext/azure-iot/iot) for a complete list of supported commands. Some IoT CLI usage tips on the [wiki](https://github.com/Azure/azure-iot-cli-extension/wiki/Tips).

#### Device Twins
(Available in the Standart tier $)
State is syncronized between "desired" and "reported" properties.

![](assets/Pasted%20image%2020210904145803.png)

### Azure IoT Central

SaaS application that provides a complete platform for hosting IoT applications. Streamline the entire lifecycle of creating and managing IoT applications. One can:
- See all devices with live data
- Manage device's properties and set values
- Set rules and workflows for different devices
See [official site for details](https://azure.microsoft.com/en-us/services/iot-central/#overview) or watch the [walkthrough for an example](https://www.youtube.com/watch?v=G32stXSwtyA).

### IoT Central vs IoT Hub

See this [excellent comparison between the two](https://docs.microsoft.com/en-us/azure/iot-develop/concepts-overview-connection-options#application-platforms-iot-central-and-iot-hub), including a table with the tools used to connect and manage devices in each one.

Video [compares Azure IoT Hub, Azure IoT Central and Azure Sphere](https://www.youtube.com/watch?v=RHkqFxJWhr8)

### Resources, Guides & Tutorials

The tutorial [Azure ESP32 IoT DevKit Get Started](https://docs.microsoft.com/en-us/samples/azure-samples/esp32-iot-devkit-get-started/sample/) features a M5Stack board but should work with other ESP32 devices

M5Stack and Azure IoT: [Run a simple C sample on M5Stack IoT Kit device running RTOS](https://github.com/Azure/azure-iot-device-ecosystem/blob/master/get_started/rtos-m5stack-c.md)

Video: [Azure ESP32 Dev Kit Board and resources](https://www.youtube.com/watch?v=nwxkUQPESCU)

Repository: [Azure Samples for Espressif (ESP) Microcontrollers](https://github.com/Azure-Samples/ESP-Samples)

## AWS

Teachers can apply to have JAC as a member institution of AWS. Teachers will receive 150$ in annual account credit and students will receive 100$. [More info here](https://www.awseducate.com/faqs?app=3#back2top).

Register JAC as a partner institution [here](https://aws.amazon.com/training/awsacademy/?nc2=sb_ep_aca)

### Data visualization service

- [AWS IoT SiteWise](https://aws.amazon.com/blogs/iot/aws-iot-sitewise-2020-in-review/)
- [AWS QuickSight](https://aws.amazon.com/quicksight/?did=ft_card&trk=ft_card)

### Data filtering and event triggering

- [AWS IoT Analytics](https://aws.amazon.com/iot-analytics/?nc=sn&loc=0)
- [AWS IoT Events](https://aws.amazon.com/iot-events/?nc2=type_a)
- [AWS Data Pipeline](https://aws.amazon.com/datapipeline/?nc2=type_a)

### Resources, Guides & Tutorials

- [IoT All the Things videos](https://aws.amazon.com/architecture/all-in-livestream-series/iot-all-the-things-special-projects/?all-in-livestream-cards.sort-by=item.additionalFields.sortDate&all-in-livestream-cards.sort-order=desc&awsf.event-type=*all&awsf.industry=*all&awsf.products=*all&awsf.tech-category=*all&awsm.page-all-in-livestream-cards=1)
- [The Internet of Things on AWS – Official Blog](https://aws.amazon.com/blogs/iot/)

