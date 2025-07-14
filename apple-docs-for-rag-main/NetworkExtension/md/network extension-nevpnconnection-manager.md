

- Network Extension
- NEVPNConnection
-  manager 

Instance Property

# manager

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 17.0+visionOS 1.0+

``` source
var manager: NEVPNManager { get }
```

## See Also

### Getting VPN connection status

var status: NEVPNStatus

The current status of the VPN connection.

enum NEVPNStatus

The possible states of a VPN connection.

var connectedDate: Date?

The date and time when the connection status changed to `NEVPNStatusConnected`.

