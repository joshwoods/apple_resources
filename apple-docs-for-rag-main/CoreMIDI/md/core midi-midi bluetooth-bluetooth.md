

- Core MIDI
-  MIDI Bluetooth 

API Collection

# MIDI Bluetooth

Connect to Bluetooth Low Energy MIDI peripherals.

## Overview

In macOS 13 or later and iOS 16 or later, the system automatically reconnects Bluetooth Low Energy (BLE) MIDI peripherals when powered on, if the device supports pairing. Previously, it was necessary to use Audio MIDI Setup to establish BLE MIDI connections.

For devices that don’t support pairing, Core MIDI can enable Core Bluetooth connections for input/output (I/O).

This API enables connection of BLE MIDI peripherals that don’t support pairing using Core Bluetooth with the following steps:

1.  Scan for and connect to a BLE MIDI peripheral.

2.  Confirm the peripheral has a BLE MIDI service.

3.  Confirm the BLE MIDI service on the peripheral has a MIDI I/O characteristic for the MIDI service.

Once a BLE MIDI peripheral connects — and you confirm that it possess both the BLE MIDI service and BLE MIDI I/O characteristic — call MIDIBluetoothDriverActivateAllConnections() to have Core MIDI enable I/O on those connections.

To disconnect a peripheral, obtain the CBUUID of the peripheral and call MIDIBluetoothDriverDisconnect(_:).

## Topics

### Managing Device Connections

func MIDIBluetoothDriverActivateAllConnections() -> OSStatus

Promote all active Bluetooth connections into an online MIDI device capable of input and output.

func MIDIBluetoothDriverDisconnect(CFString) -> OSStatus

Disconnect the Bluetooth MIDI driver from a Bluetooth Low Energy MIDI peripheral.

## See Also

### Services

MIDI Services

Communicate with hardware using Universal MIDI Packets.

MIDI System Setup

Configure the global MIDI system.

MIDI Messages

Create and configure messages.

MIDI Thru Connection

Create play-through connections between sources and destinations.

MIDI Networking

Create and manage devices connected over a local network.

MIDI Drivers

Create driver plug-ins.

MIDI Capability Inquiry

Provide support for bidirectional discovery and configuration of devices.

