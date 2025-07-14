

- Core MIDI
-  MIDI System Setup 

API Collection

# MIDI System Setup

Configure the global MIDI system.

## Overview

The primary clients of this API are apps that present a user interface to configure the global MIDI system, and MIDI drivers that dynamically modify the system state as users connect and disconnect hardware.

## Topics

### Managing Devices

func MIDISetupAddDevice(MIDIDeviceRef) -> OSStatus

Adds a driver-owned MIDI device to the current MIDI setup.

func MIDISetupRemoveDevice(MIDIDeviceRef) -> OSStatus

Removes a driver-owned MIDI device from the current MIDI setup.

### Managing External Devices

func MIDIExternalDeviceCreate(CFString, CFString, CFString, UnsafeMutablePointer&lt;MIDIDeviceRef>) -> OSStatus

Creates an external MIDI device.

func MIDISetupAddExternalDevice(MIDIDeviceRef) -> OSStatus

Adds an external MIDI device to the current MIDI setup.

func MIDISetupRemoveExternalDevice(MIDIDeviceRef) -> OSStatus

Removes an external MIDI device from the current MIDI setup.

### Managing Entities

func MIDIDeviceNewEntity(MIDIDeviceRef, CFString, MIDIProtocolID, Bool, Int, Int, UnsafeMutablePointer&lt;MIDIEntityRef>) -> OSStatus

Adds a new entity to a device.

func MIDIDeviceRemoveEntity(MIDIDeviceRef, MIDIEntityRef) -> OSStatus

Removes an entity from a device.

func MIDIEntityAddOrRemoveEndpoints(MIDIEntityRef, Int, Int) -> OSStatus

Adds or removes an entity’s endpoints.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## See Also

### Services

MIDI Services

Communicate with hardware using Universal MIDI Packets.

MIDI Bluetooth

Connect to Bluetooth Low Energy MIDI peripherals.

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

