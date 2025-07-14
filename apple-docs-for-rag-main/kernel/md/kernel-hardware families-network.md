

- Kernel
- Hardware Families
-  Network 

API Collection

# Network

Implement a driver that interacts with network interfaces such as Ethernet adaptors.

## Overview

For most types of network interfaces, the use of kernel extensions is deprecated. Instead, create a DriverKit extension using NetworkingDriverKit.

## Topics

### Interfaces

IONetworkInterface

Abstract class that manages the connection between an IONetworkController and the data link interface layer.

IONetworkController

Implements the framework for a generic network controller.

### Network Data

IONetworkData

An object that manages a fixed-size named buffer.

IONetworkMedium

An object that encapsulates information about a network medium (i.e. 10Base-T, or 100Base-T Full Duplex).

IOPacketQueue

Implements a bounded FIFO queue of mbuf packets.

IOPacketBufferConstraints

## See Also

### Interfaces

Audio

Implement a driver that interacts with audio hardware.

Graphics and Displays

Implement a driver that interacts with graphics and video hardware.

HID

Implement a driver that interacts with human interface devices, such as mice and keyboards.

SCSI

Implement a driver that supports Small Computer System Interface (SCSI) protocols.

Mass Storage

Implement a driver that communicates with CD, DVD, or other mass storage devices.

