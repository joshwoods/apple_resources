

- MatterSupport
-  MatterAddDeviceExtensionRequestHandler 

Class

# MatterAddDeviceExtensionRequestHandler

The object that handles configuration and commissioning of a device into an ecosystem.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
@objc
class MatterAddDeviceExtensionRequestHandler
```

## Mentioned in 

Adding Matter support to your ecosystem

## Overview

This class facilitates the user interface flow during the setup of a new Matter device. Subclass this class and override its methods, except for `beginRequest(with:)`. The principal class for the app’s extension declared by the NSPrincipalClass in the extension plist must inherit from this base class.

If the MatterAddDeviceRequest.Topology object in the request has two or more homes, the user interface flow displays a picker to allow selection of a home. If the object contains one home, that home is the selected home and the user interface flow doesn’t display a picker. If the object contains no home, then the user interface flow doesn’t display a picker, and any methods take a home parameter receive `nil`.

Note

Don’t call `super` within the overridden method.

## Topics

### Creating the request handler

init()

### Configuring and validating the device

func configureDevice(named: String, in: MatterAddDeviceRequest.Room?) async

Configures the device with selected attributes.

func validateDeviceCredential(MatterAddDeviceExtensionRequestHandler.DeviceCredential) async throws

Performs verification and attestation checks.

struct DeviceCredential

A collection of device credentials the device presents during commissioning.

func rooms(in: MatterAddDeviceRequest.Home?) async -> [MatterAddDeviceRequest.Room]

Provides rooms that correspond to a home in the device setup.

### Commissioning the device

func commissionDevice(in: MatterAddDeviceRequest.Home?, onboardingPayload: String, commissioningID: UUID) async throws

Commissions the device with the onboarding payload.

### Selecting the Thread network

func selectThreadNetwork(from: [MatterAddDeviceExtensionRequestHandler.ThreadScanResult]) async throws -> MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

Provides the visible Thread networks to the device.

struct ThreadScanResult

A result of a Thread-scan operation performed on the device

struct ThreadNetworkAssociation

The description of an association to a Thread network.

### Selecting the Wi-Fi network

func selectWiFiNetwork(from: [MatterAddDeviceExtensionRequestHandler.WiFiScanResult]) async throws -> MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

Provides the visible Wi-Fi networks to the Matter device.

struct WiFiScanResult

A result of a Wi-Fi-scan operation performed on the device

struct WiFiNetworkAssociation

The description of an association to a Wi-Fi network.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Adding a device

Adding Matter support to your ecosystem

Allow people to add Matter accessories to your platform.

struct MatterAddDeviceRequest

A request that adds and sets up a device into an ecosystem.

