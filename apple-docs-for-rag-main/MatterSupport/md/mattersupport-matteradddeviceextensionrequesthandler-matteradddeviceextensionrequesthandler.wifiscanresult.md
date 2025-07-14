

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  MatterAddDeviceExtensionRequestHandler.WiFiScanResult 

Structure

# MatterAddDeviceExtensionRequestHandler.WiFiScanResult

A result of a Wi-Fi-scan operation performed on the device

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct WiFiScanResult
```

## Overview

Use an instances to create a `WiFiNetworkAssociation` as a possible Wi-Fi network for the device to join.

## Topics

### Creating the result

init(ssid: Data, rssi: Int8, security: MTRNetworkCommissioningWiFiSecurity, band: MTRNetworkCommissioningWiFiBand)

Creates a new instance of the request handler.

### Getting result information

var band: MTRNetworkCommissioningWiFiBand

The band for the Wi-Fi network.

var rssi: Int8

The device-observed RSSI of the network.

var security: MTRNetworkCommissioningWiFiSecurity

The security method used to secure the Wi-Fi network.

var ssid: Data

The SSID of the Wi-Fi network.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Selecting the Wi-Fi network

func selectWiFiNetwork(from: [MatterAddDeviceExtensionRequestHandler.WiFiScanResult]) async throws -> MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

Provides the visible Wi-Fi networks to the Matter device.

struct WiFiNetworkAssociation

The description of an association to a Wi-Fi network.

