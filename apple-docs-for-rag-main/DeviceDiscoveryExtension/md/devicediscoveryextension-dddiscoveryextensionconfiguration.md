

- DeviceDiscoveryExtension
-  DDDiscoveryExtensionConfiguration 

Class

# DDDiscoveryExtensionConfiguration

An object that manages the extension’s communication with the framework.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
@MainActor @preconcurrency
class DDDiscoveryExtensionConfiguration where T : DDDiscoveryExtension
```

## Overview

Your app’s primary extension class provides a property of this type. Create the instance by calling init(discoveryExtension:) with the argument set to `self`.

## Topics

### Creating an extension configuration

init(discoveryExtension: T)

Creates an extension configuration with a reference to a specific extension.

## Relationships

### Conforms To

- AppExtensionConfiguration
- DDDiscoveryExtensionConfigurationProtocol
- Sendable

## See Also

### Extension

protocol DDDiscoveryExtension

A specification that enables the framework to start and stop the extension’s discovery process.

class DDDiscoverySession

An object that relays device discovery events from the extension to the system.

protocol DDDiscoveryExtensionConfigurationProtocol

A specification that provides a communication channel between the extension and the framework.

