# IoT Development Environments

Dev environtments under consideration for [README](README.md)

There are 3 possible development environments to use for the course:

- Arduino IDE used for the Arduino framework
- PlatformIO is framework agnostic
- ESP-IDF used for Espressif's ESP32 framework

## EDP-IDF

Open source integrated development framework created by Espressif.
Uses FreeRTOS firmware.

According to their official Get Started:

> You have a choice to either download and install the following software manually
>
> -   **Toolchain** to compile code for ESP32
>     
> -   **Build tools** - CMake and Ninja to build a full **Application** for ESP32
>     
> -   **ESP-IDF** that essentially contains API (software libraries and source code) for ESP32 and scripts to operate the **Toolchain**     
>
> **or** get through the onboarding process using the following official plugins for integrated development environments (IDE) described in separate documents
> 
> -   [Eclipse Plugin](https://github.com/espressif/idf-eclipse-plugin) ([installation link](https://github.com/espressif/idf-eclipse-plugin#installing-idf-plugin-using-update-site-url))
>     
> -   [VS Code Extension](https://github.com/espressif/vscode-esp-idf-extension) ([setup](https://github.com/espressif/vscode-esp-idf-extension/blob/master/docs/tutorial/install.md))
>

![Development of applications for ESP32](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/_images/what-you-need.png)

> **It is recommended to use the *VS Code Extension* to simplify setup**

### ESP-IDF build system

To understand the details of the different componets of a ESP-IDF project or how it is built, see the [official Build System page](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/build-system.html).

### ESP-IDF VS Code extension

YouTube Video:[ Quick User Guide for the ESP-IDF VS Code Extension](https://www.youtube.com/watch?v=Lc6ausiKvQM)

### Project Structure

The reposity [esp-idf](https://github.com/espressif/esp-idf/tree/5f38b766a83d18f78167d1d0dd8c8427ea1a36cb)/[examples](https://github.com/espressif/esp-idf/tree/5f38b766a83d18f78167d1d0dd8c8427ea1a36cb/examples)/[get-started](https://github.com/espressif/esp-idf/tree/5f38b766a83d18f78167d1d0dd8c8427ea1a36cb/examples/get-started)/**sample_project**/ shows the simplest buildable ESP-IDF example.

sample_project contains one source file `main.c` in C language. ESP-IDF projects are built using CMake and build configuration is contained in `CMakeLists.txt`.


### Arduino with ESP-IDF

Espressif provides a way to use the [Arduino framework with ESP-IDF](https://docs.espressif.com/projects/arduino-esp32/en/latest/esp-idf_component.html).

Arduino-esp32 includes libraries for Arduino compatibility along with some object wrappers around hardware specific devices.

%%TODO: Test this as a transition from Arduino IDE to VS Code with ESP-IDF%%

This should not be comfused with [using ESP32 in the Arduino IDE](https://docs.espressif.com/projects/arduino-esp32/en/latest/getting_started.html).

## Projects written in C vs C++

I don't fully understand the differences of writting and compiling projects with C vs C++.

FreeRTOS seems to be written in C.

It seems to involve the use of `extern "C"`:

```C
extern "C" void app_main()
{
 initArduino();
 pinMode(4, OUTPUT);
 digitalWrite(4, HIGH);
 //do your own thing
}
```

## ESP Rainmaker

A "framework" integrated with ESP-IDF to monitor and control IoT devices using a smartphone.

ESP-IDF VSCode Extension comes pre package with [ESP Rainmaker](https://rainmaker.espressif.com) 

See [official Get Started for details.](https://rainmaker.espressif.com/docs/get-started.html)

Great process overview with YouTube video: [ESP RainMaker](https://www.youtube.com/watch?v=Heo18HLgh9g). 

### ESP Rainmaker with Arduino IDE

Blog post describes [how to use Rainmaker with the Arduino IDE](https://blog.espressif.com/esp-rainmaker-now-in-arduino-cf1474526172

## Micropython

### Micropython with M5Core2
 
 The M5Stack company pushes the use of [Ui-Flow](https://shop.m5stack.com/pages/uiflow) for writting code for the M5Core2.
 The community is pushing M5Stack and working on writing pure Micropython code for the M5Core2.
 
 See[ this discussion in the M5Stack community forums ](https://community.m5stack.com/topic/2601/pure-micro-python-without-ui-flow-on-my-m5stack-core2)for info on how to use Micropython with the M5Core2

### Azure IoTCentral SDK for Micropython

[This repository ](https://github.com/iot-for-all/iotc-micropython-client)
contains code for the Azure IoT Central SDK for Micropython. This enables micropython developers to easily create device solutions that semealessly connect to Azure IoT Central applications.

## LVGL

LittlevGL (recently named LVGL) is a high-level GUI library, it’s implemented in C and its API is in C. This library speeds up the creating of user interfaces for microcontrollers.

### LVGL with Micropython

Although LVGL uses an API in C, it provides bindings in Micropython.
See [this repo for more details](https://github.com/lvgl/lv_micropython/).

[This blog post provides an exelent overview and demo](https://blog.lvgl.io/2019-02-20/micropython-bindings) of using LVGL and Micropython together.

## Pure C++

[Compiler Explorer](https://godbolt.org/): shows C++ code compiled to assembly according to a specified compiler