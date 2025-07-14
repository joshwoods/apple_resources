

- System Configuration
-  SCNetworkConnectionStatus 

Enumeration

# SCNetworkConnectionStatus

The current status of the network connection.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum SCNetworkConnectionStatus
```

## Overview

This status is intended to be generic and high level. An extended status, specific to the type of network connection, is also available for applications that need additonal information.

## Topics

### Constants

case invalid

The network connection refers to an invalid service.

case disconnected

The network connection is disconnected.

case connecting

The network connection is connecting.

case connected

The network connection is connected.

case disconnecting

The network connection is disconnecting.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum SCNetworkConnectionPPPStatus

The PPP-specific status of the network connection.

Statistics Dictionary Keys

Keys associated with values in the statistics dictionary.

Selection Options Dictionary Keys

Keys used with the SCNetworkConnectionCopyUserPreferences(_:_:_:) selection options dictionary.

