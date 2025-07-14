

- DeviceDiscoveryExtension
-  DDDiscoveryExtensionConfigurationProtocol 

Protocol

# DDDiscoveryExtensionConfigurationProtocol

A specification that provides a communication channel between the extension and the framework.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOSvisionOS

``` source
protocol DDDiscoveryExtensionConfigurationProtocol : AppExtensionConfiguration
```

## Overview

The DDDiscoveryExtensionConfiguration class adopts this protocol. For an example, see `Appex.swift` in Discovering a third-party media-streaming device.

## Relationships

### Inherits From

- AppExtensionConfiguration
- Sendable

### Conforming Types

- DDDiscoveryExtensionConfiguration

## See Also

### Extension

protocol DDDiscoveryExtension

A specification that enables the framework to start and stop the extension’s discovery process.

class DDDiscoverySession

An object that relays device discovery events from the extension to the system.

class DDDiscoveryExtensionConfiguration

An object that manages the extension’s communication with the framework.

