# LiquidIoT Project

This is the official repository for LiquidIoT Project (http://lively.cs.tut.fi/LiquidIoT.html). LiquidIoT project is a research done in Pervasive Computing laboratory at Tampere Universcity of Technology in collaboration with Nokia Technologies. This is 

## Introduction

LiquidIoT has three main components. The first component is an application framework for developing IoT applications. The framework is supported by a browser-based Integrated Development Environment (IDE). This IDE also supports deployment and management of the IoT applications. The second component is Runtime Environment that turns IoT devices into application servers that can run IoT applications. The last component is a Resource Registry (RR) mechanism to keep track of available IoT resources including devices and applications.

![overview](https://cloud.githubusercontent.com/assets/5477534/22821178/a036e85e-ef82-11e6-908a-705941177e09.jpg)

The above Figure illustrates the different components and operation of our platform and tool. The steps are as the following:

1. When a new device is installed, it is registered with the Resource Registry (RR) Server. This server keeps track of all known devices.

2. A new application is developed or found among pre-existing applications.

3. Suitable device(s) are discovered from RR.

4. The application is deployed to the discovered device via Application Management APIs provided by Runtime Environment.

5. The deployment result is returned to the development tool, and in a case of successful deployment the installed application is registered to the RR, too.

6. The developer tool or any other entity can search applications from RR.

7. The tool can be used for monitoring and management of the application, and

8. The result of applications' management (e.g. stopping, starting, deleting, ert.) will be reported to both IDE and RR. 

## Directory Layout

This repository is the parent repo that includes three folders each of them pointing to one component described in Introduction Section.
    
    LiquidIoT-ApplicationFramework/         --> points to the Github repo hosting Application Framework component
    Liquid-IoT-RuntimeEnvironemnt/           --> points to the Github repo hosting Runtime Environment component
    LiquidIoT-ResourceRegistry/           --> points to the Github repo hosting Resource Registry component

## How to run

There are two main ways to run the component you want:

1. Directly going to the Github repo for the component you want to run. If you click the component folder it redirects you the Github Repo hosting the components.

2. Clone this repo. Run ```git submodule update --init <specific relative path to submodule>``` to get the latest version of the component you want to run. Then navigate to the folder assoiated with the component. Follow its README file.

## License

This project is under BSD License.
