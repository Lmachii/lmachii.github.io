---
layout: project
type: project
image: images/Capture1.PNG
title: Modular IoT Hydroponics
permalink: projects/hydroponics
# All dates must be YYYY-MM-DD format!
date: 2016-09-01
labels:
  - Node Red
  - Arduino
  - JavaScript
  - Raspberry Pi
summary: I worked with the REDlab group to design and create a semi-automated modular hydroponics system.
---

Hydroponics is the method of growing plants while using a different medium to grow in as well as a highly monitored and unconventional watering method.  For our specific hydroponics project we utilized the ebb and flow method.  We also used small rocks as our medium to grow our plants.  The water would rise up to about the height of the containers, stay there for a few minutes, and then drain all the water out of the containers.  Hydroponics is an effect way of growing plants because it maximizes the amount of oxygen that a plant can absorb. 

We designed a control system that used a raspberry pi as a main hub of the system.  This would with in pair with an arduino as a micro-controller which would gather, parse, and send data to the raspberry pi.  The raspberry pi would then send the data to a server via MQTT(Message Query Telemetry Transport) which would be running a PostGRES SQL database to log and store data.  The server would send the information back to the raspberry pi via MQTT and the raspberry pi would process the data and display it onto a web page that could be accessed through the internet.  This topology was made possible through node red which is a drag-and-drop type of IDE which utilizes JavaScript functionality.
