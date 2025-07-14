

- Core WLAN
-  CWMutableConfiguration 

Class

# CWMutableConfiguration

Encapsulates a mutable configuration for an AirPort WLAN interface.

macOS 10.6+

``` source
class CWMutableConfiguration
```

## Overview

Use this class to change configuration settings or the preferred networks list. To commit configuration changes, use commitConfiguration(_:authorization:).

## Topics

### Configuring Preferred Networks

var networkProfiles: NSOrderedSet

The preferred networks list.

### Configuring Settings

var rememberJoinedNetworks: Bool

A Boolean value that determines whether to remember all joined Wi-Fi networks unless the user specifies otherwise when joining a particular Wi-Fi network.

var requireAdministratorForAssociation: Bool

A Boolean value that determines whether to require an administrator password to change networks.

var requireAdministratorForPower: Bool

A Boolean value that determines whether to require an administrator password to change the interface power state.

var requireAdministratorForIBSSMode: Bool

A Boolean value that determines whether to require an administrator password to create a computer-to-computer network.

Deprecated

## Relationships

### Inherits From

- CWConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Classes

class CWChannel

Encapsulates an IEEE 802.11 channel.

class CWConfiguration

Encapsulates an immutable configuration for an AirPort WLAN interface.

class CWInterface

Encapsulates an IEEE 802.11 interface.

class CWMutableNetworkProfile

Encapsulates a mutable network profile entry.

class CWNetwork

Encapsulates an IEEE 802.11 network, providing read-only accessors to various properties of the network.

class CWNetworkProfile

Encapsulates an immutable network profile entry.

class CWWiFiClient

A wrapper around the entire Wi-Fi subsystem that you use to access interfaces and set up event notifications.

