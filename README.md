# Awesome Core Flight System (cFS)

This is a curated list of cFS links, apps, tools, documentation, training, misions/projects. The goal is to have a one stop shot for new and experienced users to find sources for cFS.

[Please contribute!](contributing.md)

## Table of Contents

- [Awesome Core Flight System (cFS)](#awesome-core-flight-system-cfs)
  - [Table of Contents](#table-of-contents)
  - [Framework and Development Environments](#framework-and-development-environments)
    - [cFS Home](#cfs-home)
    - [Framework Components](#framework-components)
    - [Development Environments, Distributions and Platforms](#development-environments-distributions-and-platforms)
  - [Apps](#apps)
    - [Standard Apps](#standard-apps)
    - [Lab and Sim Apps](#lab-and-sim-apps)
    - [Sample and Skeleton Apps](#sample-and-skeleton-apps)
    - [Hardware Specific Apps and Demos](#hardware-specific-apps-and-demos)
    - [Data Interface Apps](#data-interface-apps)
  - [Tools](#tools)
  - [Platforms and Demos](#platforms-and-demos)
  - [Documentation](#documentation)
    - [Reference Documentation and User's Guides](#reference-documentation-and-users-guides)
    - [Applications](#applications)
    - [Articles](#articles)
    - [Ground Systems](#ground-systems)
    - [Overviews and Training](#overviews-and-training)
    - [Verification and Validation](#verification-and-validation)
  - [cFS Spacecraft, Payloads and Projects](#cfs-spacecraft-payloads-and-projects)
    - [Currently Flying Spacecraft](#currently-flying-spacecraft)
    - [Upcoming Missions/Spacecraft](#upcoming-missionsspacecraft)
    - [Past Missions/Spacecraft](#past-missionsspacecraft)
    - [Prototypes](#prototypes)

## Framework and Development Environments

### cFS Home

- [NASA cFS Home](https://cfs.gsfc.nasa.gov/) - NASA's homepage to cFS
- [NASA cFS Bundle](https://github.com/nasa/cFS) - NASA's GitHub home to cFS

### Framework Components

- [cFE](https://github.com/nasa/cFE) - Core Flight Executive
- [OSAL](https://github.com/nasa/osal/) - Operating System Abstraction Level
- [PSP](https://github.com/nasa/PSP/) -Platform Support Package

### Development Environments, Distributions and Platforms


- [cfs-basecamp](https://github.com/cfs-tools/cfs-basecamp) - A lightweight environment to help learn cFS.
- [nos3](https://github.com/nasa/nos3) - Small satellite enivronment with cFS, COSMOS and NOS3 simulator
- [OpenSatKit](https://github.com/OpenSatKit/OpenSatKit) - Includes cFS, COSMOS Ground System and the 42 Simulator.
- [pi-sat](https://github.com/OpenSatKit/pi-sat) - A cFS distribution that can be run on a Raspberry Pi.

## Apps

### Standard Apps
 
- [CS](https://github.com/nasa/CS) - The Checksum (CS) application is used for for ensuring the integrity of onboard memory.
- [CF](https://github.com/nasa/CF) - The CF application provides CFDP CCSDS File Delivery Protocol services.
- [CI](https://github.com/nasa/CFS_CI) - The Command Ingest (CI) application receives commands and forwards the command to the appropriate application over the software bus.
- [DS](https://github.com/nasa/DS) - The Data Storage (DS) application is used for storing software bus messages into files.
- [FM](https://github.com/nasa/FM) - The File Management (FM) application provides onboard file system management services.
- [HK](https://github.com/nasa/HK) - The Housekeeping (HK) application is used for building and sending combined telemetry messages to the software bus for routing.
- [HS](https://github.com/nasa/HS) - The Healthy and Safety (HS) application provides functionality for miscellaneous different monitoring, servicing and reporting.
- [LC](https://github.com/nasa/LC) - The Limit Checking (LC) application monitors telemetry data, compares the values against predefined threshold limits and supports predefined responses.
- [MD](https://github.com/nasa/MD) - The Memory Dwell (MD) application monitors memory addresses accessed by the CPU.
- [MM](https://github.com/nasa/MM) - The Memory Manager (MM) application is used for the loading and dumping system memory.
- [SBN](https://github.com/nasa/SBN) - The Software Bus Networks (SBN) application connects the cFE Software Bus (SB) to other buses.
- [SC](https://github.com/nasa/SC) - The Stored Command (SC) application allows a system to be autonomously commanded using sequences of commands that are preloaded.
- [SCA](https://github.com/nasa/SCA) - The Stored Absolute Command (SCA) application allows a system to be commanded 24 hours a day using sequences of absolute time tagged sequences.
- [SCH](https://github.com/nasa/SCH) - The Scheduler (SCH) application provides a method of generating software bus messages at pre-determined timing intervals.
- [TO](https://github.com/nasa/CFS_TO) - The Telemetry Output (TO) application is responsible for transmitting telemetry to external destination(s) over transport devices(s).

### Lab and Sim Apps

- [bc42_ctrl](https://github.com/cfs-apps/bc42_ctrl) - Executes a 42 Simulator spacecraft control algorithm that has been ported from 42.
- [bc42_intf](https://github.com/cfs-apps/bc42_intf) - Provide an interface between a 42 Simulator socket and the cFS Software Bus.
- [bc42_lib](https://github.com/cfs-apps/bc42_lib) - Encapsulates 42 simulator data types and functions as a single cFS library.
- [CI_LAB](https://github.com/nasa/ci_lab) - This Command Ingest Lab (CI_LAB) application is a non-flight utility to send commands to the software bus.
- [pl_sim](https://github.com/cfs-apps/pl_sim) - Payload simulator app that provides a ground interface to the payload simulator library (PL_SIM).
- [pl_sim_lib](https://github.com/cfs-apps/pl_sim_lib) - Payload simulator library that simulates a fictitious detector that provides text data.
- [SCH_LAB](https://github.com/nasa/sch_lab/) -This lab application is a non-flight packet scheduler application for the cFS Bundle.
- [TO_LAB](https://github.com/nasa/to_lab) - This lab application is a non-flight utility to downlink telemetry from the cFS Bundle.
- [TVSIO](https://github.com/nasa/tvsio) - This application provides two-way communication between cFS's Software Bus Network (SBN) and Trick simulations.
- [TVSIO Demo](https://github.com/nasa/tvsio-demo) - A sample project for integrating TVS-IO into cFS
- [sc_sim](https://github.com/cfs-apps/sc_sim) - Simulate a simple spacecraft operational interface that exposes users to a remote operational interface. 

### Sample and Skeleton Apps

- [Sample App](https://github.com/nasa/sample_app/) - This sample application is a non-flight example application implementation for the cFS Bundle.
- [Skeleton App](https://github.com/nasa/skeleton_app) - A bare-bones cFS application

### Hardware Specific Apps and Demos

- [berry_imu](https://github.com/cfs-apps/berry_imu) - Core Flight System app that interfaces to the Ozzmaker Berry IMU over a Raspberry Pi I2C interface.
- [gpio_demo](https://github.com/cfs-apps/gpio_demo) - Example app controlling a GPIO pin that can be used as a starting point for more sophisticated apps.
- [lora](https://github.com/cfs-apps/lora) - Long Range (LoRa) radio communication tech demo app using a Durand/Packard 2400 MHz link.
- [lora_rx](https://github.com/cfs-apps/lora_rx) - Long Range (LoRa) Receive app for a tech demo of a Durand/Packard 2400 MHz link. 
- [lora_tx](https://github.com/cfs-apps/lora_tx) - Long Range (LoRa) Transmit app for a tech demo of a Durand/Packard 2400 MHz link.
- [pi_iolib](https://github.com/cfs-apps/pi_iolib) - cFS library providing an interface to Raspberry Pi peripherals
- [rpi_btn](https://github.com/cfs-apps/rpi_btn) - Raspberry Pi app demonstrating how to interface with a button.
- [sx128x](https://github.com/cfs-apps/sx128x) - An SX1280 transceiver library design to be used on a Raspberry Pi.

### Data Interface Apps
- [jmsg_app](https://github.com/cfs-apps/jmsg_app) - Serves as a ground command and telemetry interface for the JMSG_LIB.
- [jmsg_lib](https://github.com/cfs-apps/jmsg_lib) - Provide tools for bi-directional translation between JSON text messages and cFS Software Bus binary messages.
- [jmsg_mqtt](https://github.com/cfs-apps/jmsg_mqtt) - Provide a gateway between the cFS Software Bus messages and MQTT messages. The initial version supports predefined MQTT JSON payloads.
- [jmsg_udp](https://github.com/cfs-apps/jmsg_udp) - Provide a gateway between the cFS Software Bus and JSON messages transmitted using UDP.
- [mqtt_lib](https://github.com/cfs-apps/mqtt_lib) - The Eclipse Paho Embedded C MQTT Library ported to the core Flight System.
- [pl_mgr](https://github.com/cfs-apps/pl_mgr) - Example payload management app.
- [tbl_sat]() - Raspberry Pi app used in the Table Sat kit.
- [tplug_web]() - Serves as an example for using JMSG_MQTT to interface with a web app via an MQTT broker. 

## Tools

- [cFS-GroundSystem](https://github.com/nasa/cFS-GroundSystem) - Default ground system included with NASA's cFS.
- [elf2cfetbl](https://github.com/nasa/elf2cfetbl) - A ground utility to convert ELF to cFE binary tables for cFS.
- [tblCRCTool](https://github.com/nasa/tblCRCTool) - A ground utility to generate binary table CRCs for cFS.

## Platforms and Demos

- [rtems-cfs-demo](https://github.com/alanc98/rtems-cfs-demo) - This is a Beaglebone Black RTEMS core Flight System demo.

## Documentation

### Reference Documentation and User's Guides

  - [cFE User's Guide](https://github.com/nasa/cFS/blob/gh-pages/cfe-usersguide.pdf)
  - [OSAL User's Guide](https://github.com/nasa/cFS/blob/gh-pages/osal-apiguide.pdf)
  - [cFE App Developer's Guide](https://github.com/nasa/cFE/blob/main/docs/cFE%20Application%20Developers%20Guide.md)


### Applications

- [Core Flight Software Projects on Orion Multi-Purpose Crew Vehicle](https://ntrs.nasa.gov/citations/20190000011) (2018)
- [Application of the Core Flight System to a Lunar Rover](https://ntrs.nasa.gov/citations/20170012168) (2017)
- [Future Standardization of Space Telecommunications Radio System with Core Flight System](https://ntrs.nasa.gov/citations/20170001293) (2016)
- [Lessons from 30 Years of Flight Software](https://ntrs.nasa.gov/citations/20150019915) (2015)
- [NASA's Core Flight Software - A Reusable Real-Time Framework](https://ntrs.nasa.gov/citations/20140017040) (2014) - Includes cFS overview, Morpheus Lander case status, etc

### Articles

- [The Road to the New Flight Software](https://cfs.gsfc.nasa.gov/Issue%2051Summer%202013.pdf) - Starting on page 33
- [Open Source Space](https://www.linuxjournal.com/content/open-source-space?page=0,0) - Linux Journal

### Ground Systems

- [cFS Ground System Guide](https://github.com/nasa/cFS-GroundSystem/blob/main/Guide-GroundSystem.md)
- [OpenC3 COSMOS Guide](https://docs.openc3.com/docs/guides/cfs)

### Overviews and Training

- [cFE/CFS (Core Flight Executive/Core Flight System)](https://ntrs.nasa.gov/citations/20090005965) (2008)
- [CFS-101](https://github.com/nasa/CFS-101) - Note that this training is deprecated but it is a core training provided by NASA.
- [cFS Overview](https://cfs.gsfc.nasa.gov/cFS-OviewBGSlideDeck-ExportControl-Final.pdf)
- [Core Flight System (cFS) Training - cFS Caelum](https://ntrs.nasa.gov/citations/20210022378) (2021)
- [Core Flight System (cFS) Training](https://ntrs.nasa.gov/citations/20205000691) (2020)
- [Open Mission Stack Learn Page](https://openmissionstack.com/learn)


### Verification and Validation

- [Open Source Core Flight System (cFS) Flight Software (FSW) Verification & Validation (V&V) Final Summary: IV&V Analysis Technical Report](https://ntrs.nasa.gov/citations/20205010026) (2020)
- [Verifying Architectural Design Rules of the Flight Software Product Line](https://ntrs.nasa.gov/citations/20090016208) (2009)


## cFS Spacecraft, Payloads and Projects

The following projects are documented or reported as using cFS.

### Currently Flying Spacecraft

- [LRO](https://science.nasa.gov/mission/lro/) - Lunar Reconnaissance Orbitor
- [GPM](https://gpm.nasa.gov/missions/GPM) - Global Precipitation Measurement
- [MMS](https://science.nasa.gov/mission/mms) - Magnetospheric Multiscale
- [PSP](https://science.nasa.gov/mission/parker-solar-probe/) - Parker Solar Probe

### Upcoming Missions/Spacecraft

- [Artemis II Orion](https://www.nasa.gov/mission/artemis-ii/) - Similar use as Artemis I including camera controllers and backup flight software.

### Past Missions/Spacecraft

- [Artemis I Orion](https://www.nasa.gov/mission/artemis-i/) - Used in camera controllers and backup flight software per NASA presentation: [Core Flight Software Projects on Orion Multi-Purpose Crew Vehicle](https://ntrs.nasa.gov/citations/20190000011).
- [Ascent Abort 2 (AA-2)](https://www.nasa.gov/mission/ascent-abort-2/) - Used as primary flight control system per NASA presentation: [Core Flight Software Projects on Orion Multi-Purpose Crew Vehicle](https://ntrs.nasa.gov/citations/20190000011). 
- [LADEE](https://science.nasa.gov/mission/ladee) - Lunar Atmosphere and Dust Environment Explorer
- [Van Allen Probes (formerly RBSP)](https://en.wikipedia.org/wiki/Van_Allen_Probes)

### Prototypes

- [Project Morpheus](https://en.wikipedia.org/wiki/Project_Morpheus) - A full scale robotic lander used as a risk reduction test article
