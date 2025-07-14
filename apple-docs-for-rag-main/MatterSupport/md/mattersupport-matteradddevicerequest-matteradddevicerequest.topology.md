

- MatterSupport
- MatterAddDeviceRequest
-  MatterAddDeviceRequest.Topology 

Structure

# MatterAddDeviceRequest.Topology

Information describing the properties of the ecosystem.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct Topology
```

## Overview

The topology of a fabric consists of its homes, rooms, and devices. The number of homes included in this class determines whether the setup presents a home selection step. If there are two or more homes, the user selects one home to add the device to.

## Topics

### Creating the topology

init(from: any Decoder) throws

Create the request from a decoder.

init(ecosystemName: String, homes: [MatterAddDeviceRequest.Home])

Creates the topology.

### Getting the properties

var ecosystemName: String

The name of your ecosystem.

var homes: [MatterAddDeviceRequest.Home]

An array of available homes to add the new device into.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Setting up the request

struct Home

The representation of a home that appears in the picker during device setup.

struct Room

The representation of a room that appears in the picker during device setup.

var setupPayload: MTRSetupPayload?

The payload to use for Matter device setup.

var topology: MatterAddDeviceRequest.Topology

A configuration object representing the topology of the initiating ecosystem.

