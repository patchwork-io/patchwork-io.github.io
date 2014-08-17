---
layout: page
title: ABOUT
permalink: /about/
---

### {{ site.tagline }}

Patchwork is a toolkit for connecting various devices into a network of things or, in a more broad case - Internet of Things (IoT). The main goal of creating this toolkit is having a lightweight set of components that can help to quickly integrate different devices (i.e. Arduinos, RaspberryPI's, Plugwise, etc) into a smart environment and expose specific devices' capabilities as RESTful/SOAP/CoAP/MQTT/etc services.

It allows to harmonize the various low-level APIs and provide an application developer with a simple access to the devices.

If you have sensors reporting their data via gpio interface, or via USB or serial port, or a custom home automation
system that provides data and accept control commands via propriatory XML-RPC interface, with Patchwork Toolkit you
can connect all those devices with Patchwork Device Gateway (DGW) and have standard API for your applications. 
Besides, Patchwork Toolkit provides a Device Resources Catalog (DC) so you have a central storage for resources descriptions 
of all available devices (metrics, data sources, etc). The DC is discoverable via DNS-SD (Bonjour) protocol therefore 
you application does not need to hardcode all the endpoints.
Additionally Patchwork Toolkit provide a Services Catalog (SC), which is a directory of services in your network of things. 
All DC are registered in SC by default. Additional services (including your own) can be placed there as well.

Patchwork is completey written in [Go](http://golang.org) programming language. Although integration of devices can be done in any other language of your choice.

It is crossplatform - majour platforms are supported, such as OSX, Linux, Windows (tested on Windows 7).
The Patchwork Toolkit can be installed (well tested) on RaspberryPI and BeagleBone boards as well.
