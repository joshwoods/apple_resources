

- DeviceDiscoveryExtension
-  DDDiscoverySession 

Class

# DDDiscoverySession

An object that relays device discovery events from the extension to the system.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
class DDDiscoverySession
```

## Overview

The system passes the extension an instance of this class when it attempts to discover a device. Device discovery starts when an app displays AVRoutePickerView and the system calls the extension’s `startDiscovery(session:)` implementation.

## Topics

### Providing an event to the system

func report(DDDeviceEvent)

Reports an event to the system.

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

### Extension

protocol DDDiscoveryExtension

A specification that enables the framework to start and stop the extension’s discovery process.

class DDDiscoveryExtensionConfiguration

An object that manages the extension’s communication with the framework.

protocol DDDiscoveryExtensionConfigurationProtocol

A specification that provides a communication channel between the extension and the framework.

