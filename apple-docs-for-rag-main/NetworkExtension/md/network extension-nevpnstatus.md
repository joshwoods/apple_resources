

- Network Extension
-  NEVPNStatus 

Enumeration

# NEVPNStatus

The possible states of a VPN connection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNStatus
```

## Overview

After the VPN transitions from the NEVPNStatus.disconnected to the NEVPNStatus.disconnecting state, the system doesn’t close TCP connections, but ignores packets to and from established network connections. When the VPN transitions to another state — for example, from a Wi-Fi to a cellular network — the system ignores network traffic and the VPN client typically reconnects to the VPN server.

## Topics

### Statuses

case disconnecting

The VPN is in the process of disconnecting.

case reasserting

The VPN is in the process of reconnecting.

case connected

The VPN is connected.

case connecting

The VPN is in the process of connecting.

case disconnected

The VPN is disconnected.

case invalid

The associated VPN configuration doesn’t exist in the Network Extension preferences or isn’t enabled.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting VPN connection status

var manager: NEVPNManager

var status: NEVPNStatus

The current status of the VPN connection.

var connectedDate: Date?

The date and time when the connection status changed to `NEVPNStatusConnected`.

