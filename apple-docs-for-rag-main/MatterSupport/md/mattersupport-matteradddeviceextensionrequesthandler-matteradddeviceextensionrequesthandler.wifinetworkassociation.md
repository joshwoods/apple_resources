

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation 

Structure

# MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

The description of an association to a Wi-Fi network.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct WiFiNetworkAssociation
```

## Topics

### Getting network information

static var defaultSystemNetwork: MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

The current Wi-Fi network of the iOS device.

static func network(ssid: Data, credentials: Data) -> MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

Maintains information about a specific Wi-Fi network.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Selecting the Wi-Fi network

func selectWiFiNetwork(from: [MatterAddDeviceExtensionRequestHandler.WiFiScanResult]) async throws -> MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

Provides the visible Wi-Fi networks to the Matter device.

struct WiFiScanResult

A result of a Wi-Fi-scan operation performed on the device

