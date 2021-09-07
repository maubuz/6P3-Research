# Hardware under consideration

## M5Stack Core 2 - AWS EduKit

See a [demo of the kit here](https://www.youtube.com/watch?v=GEnZX2_mFMM). 

- Azure certified. [Details here](https://devicecatalog.azure.com/devices/b701b555-d3e6-439f-4d41-e6b71a580dc8)
- AWS certified for IoT education purposes
- Espressif Esp32
  - Hardware security certificate buildt-in via Microchip ATECC608 Trust&GO secure element
  - Alexa capable
  - Multiple sensors
  - Built-in battery
  - Supports programing with FreeRTOS, Arduino, Micropython
- Can be purchased at:
  - [Digi-key.ca for 67.43$ CAD](https://www.digikey.ca/en/products/detail/m5stack-technology-co-ltd/K010-AWS/13562927?s=N4IgTCBcDaIMIHsBOBTMACAZs9BBA6gMroCSCAKugKIAmArgNICWALiALoC%2BQA)
  - [M5Stack store for 49.90$ US](https://shop.m5stack.com/products/m5stack-core2-esp32-iot-development-kit-for-aws-iot-edukit)
  - [Roboshop for 64.78$ CAD](https://www.robotshop.com/ca/en/m5stack-core2-esp32-iot-development-kit.html)
- Official AWS [educational documentation](https://edukit.workshop.aws/en/getting-started.html) for the kit
- [Github for M5Stack's Core 2 AWS IoT EduKit](https://github.com/m5stack/Core2-for-AWS-IoT-EduKit) contains the code and a great overview of what will be done in the education guides

### Azure IoT examples
M5Stack and Azure IoT: [Run a simple C sample on M5Stack IoT Kit device running RTOS](https://github.com/Azure/azure-iot-device-ecosystem/blob/master/get_started/rtos-m5stack-c.md)

## Seeed Wio Terminal

- Arm SAMD51 framework
- IMU(LIS3DHTR), Microphone, Buzzer, microSD card slot, Light sensor, and Infrared Emitter(IR 940nm)
- No battery included
- Azure certified device. [Details here, include quick guide for Azure IoT Hub](https://devicecatalog.azure.com/devices/8b9c5072-68fd-4fc3-8e5f-5b15e3a20bd9).

### Azure IoT Wio examples

Video: [Microsoft Azure IoT Central with IoT Plug and Play](https://www.youtube.com/watch?v=2M4bZyadxXA)

[This repository](https://github.com/SeeedJP/wioterminal-aziot-example) contains a sample application showing how to connect a Wio Terminal to Azure IoT Hub to send telemetry and receive commands.