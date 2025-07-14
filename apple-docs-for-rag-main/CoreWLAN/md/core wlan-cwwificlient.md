

- Core WLAN
-  CWWiFiClient 

Class

# CWWiFiClient

A wrapper around the entire Wi-Fi subsystem that you use to access interfaces and set up event notifications.

macOS 10.10+

``` source
class CWWiFiClient
```

## Overview

Wi-Fi client objects are heavy. Therefore, it’s more efficient to use a single, long-running client instance, rather than creating several short-lived instances. For convenience, you can use the singleton instance returned by the shared() class method.

Instead of instantiating CWInterface objects directly, use the ones provided by the instance methods of this class. For example, the interface() method returns the default Wi-Fi interface.

## Topics

### Getting the Shared Instance

class func shared() -> CWWiFiClient

The shared Wi-Fi client object.

### Initializing a Wi-Fi Client

init()

Initializes a Wi-Fi client object.

### Setting a Delegate

var delegate: AnyObject?

An object that provides Wi-Fi event handling.

### Getting Interfaces

func interface() -> CWInterface?

Returns the default Wi-Fi interface.

func interface(withName: String?) -> CWInterface?

Returns the Wi-Fi interface with the given name.

func interfaces() -> [CWInterface]?

Returns all available Wi-Fi interfaces.

class func interfaceNames() -> [String]?

Returns the list of the names of available Wi-Fi interfaces.

Deprecated

### Monitoring Events

func startMonitoringEvent(with: CWEventType) throws

Register for specific Wi-Fi event notifications.

func stopMonitoringAllEvents() throws

Unregister for all Wi-Fi event notifications.

func stopMonitoringEvent(with: CWEventType) throws

Unregister for specific Wi-Fi event notifications.

### Instance Methods

func interfaceNames() -> [String]?

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

### Classes

class CWChannel

Encapsulates an IEEE 802.11 channel.

class CWConfiguration

Encapsulates an immutable configuration for an AirPort WLAN interface.

class CWInterface

Encapsulates an IEEE 802.11 interface.

class CWMutableConfiguration

Encapsulates a mutable configuration for an AirPort WLAN interface.

class CWMutableNetworkProfile

Encapsulates a mutable network profile entry.

class CWNetwork

Encapsulates an IEEE 802.11 network, providing read-only accessors to various properties of the network.

class CWNetworkProfile

Encapsulates an immutable network profile entry.

