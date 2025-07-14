

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  MatterAddDeviceExtensionRequestHandler.ThreadScanResult 

Structure

# MatterAddDeviceExtensionRequestHandler.ThreadScanResult

A result of a Thread-scan operation performed on the device

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct ThreadScanResult
```

## Overview

Use one of these instances to create a MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation as a possible Thread network for the device to join.

## Topics

### Creating the result

init(networkName: String, panID: UInt16, extendedPANID: UInt64, channel: UInt16, extendedAddress: Data, rssi: Int8, version: UInt8, linkQualityIndicator: UInt8)

Create the extension request handler.

### Getting result information

var channel: UInt16

The Thread network radio channel.

var extendedAddress: Data

The identifier of an active Thread network Border Agent.

var extendedPANID: UInt64

The Thread network extended PAN identifier.

var linkQualityIndicator: UInt8

A receive quality indicator, as specified by Matter specification.

var networkName: String

The Thread network name.

var panID: UInt16

The Thread network PAN identifier.

var rssi: Int8

The observed RSSI of the network by the device.

var version: UInt8

The version field, as specified by the Matter specificaiton.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Selecting the Thread network

func selectThreadNetwork(from: [MatterAddDeviceExtensionRequestHandler.ThreadScanResult]) async throws -> MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

Provides the visible Thread networks to the device.

struct ThreadNetworkAssociation

The description of an association to a Thread network.

