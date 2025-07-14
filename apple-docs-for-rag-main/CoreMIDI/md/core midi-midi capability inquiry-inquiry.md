

- Core MIDI
-  MIDI Capability Inquiry 

API Collection

# MIDI Capability Inquiry

Provide support for bidirectional discovery and configuration of devices.

## Overview

MIDI Capability Inquiry (MIDI-CI) uses bidirectional communication to enable devices to exchange information about their capabilities and automatically configure themselves to work together. MIDI-CI discovers and configures devices using the following means:

- Profile configuration. Profiles define a standard set of rules for how devices respond to MIDI messages. For example, devices that support a piano profile respond to messages common to a piano, such as note on and off, velocity, and pedaling.

- Property exchange. Devices can use a set of System Exclusive (SysEx) messages to find and control various properties of other devices.

- Protocol negotiation. MIDI 2.0 devices can select between using the MIDI 1.0 or 2.0 protocols, falling back to 1.0 when not supported by other devices.

MIDI-CI defines two roles in the communication between devices: *initiator* and *responder*. Client processes acting as the initiator use the MIDICISession API, which allows for profile and property configuration of the associated responder. Client processes that advertise their own profile and property capabilities use the MIDICIResponder API, which sends responder-originated messages to initiators.

## Topics

### Capability Inquiry

class MIDICIDiscoveryManager

A singleton object that performs systemwide MIDI-CI discovery.

Deprecated

class MIDICISession

An object that represents a MIDI-CI session.

Deprecated

class MIDICIProfile

A mapping of MIDI messages to specific sounds and synthesis behaviors, such as General MIDI, a drawbar organ, and so on.

class MIDICIProfileState

An object that provides the enabled and disabled profiles for a MIDI channel or port on a device.

class MIDICIResponder

An object that responds to MIDI-CI inquiries from an initiator on behalf of a MIDI client, and handles profile and property exchange operations.

Deprecated

## See Also

### Services

MIDI Services

Communicate with hardware using Universal MIDI Packets.

MIDI System Setup

Configure the global MIDI system.

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

