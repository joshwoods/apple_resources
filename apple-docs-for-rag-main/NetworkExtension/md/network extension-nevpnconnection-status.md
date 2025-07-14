

- Network Extension
- NEVPNConnection
-  status 

Instance Property

# status

The current status of the VPN connection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var status: NEVPNStatus { get }
```

## See Also

### Getting VPN connection status

var manager: NEVPNManager

enum NEVPNStatus

The possible states of a VPN connection.

var connectedDate: Date?

The date and time when the connection status changed to `NEVPNStatusConnected`.

