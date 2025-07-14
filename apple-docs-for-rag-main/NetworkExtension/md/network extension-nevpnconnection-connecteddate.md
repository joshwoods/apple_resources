

- Network Extension
- NEVPNConnection
-  connectedDate 

Instance Property

# connectedDate

The date and time when the connection status changed to `NEVPNStatusConnected`.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var connectedDate: Date? { get }
```

## Discussion

This property contains the date and time when the connection status changed to `NEVPNStatusConnected` after previously being set to `NEVPNStatusDisconnected`. This property is set to nil whenever the status changes to `NEVPNStatusDisconnected`.

## See Also

### Getting VPN connection status

var manager: NEVPNManager

var status: NEVPNStatus

The current status of the VPN connection.

enum NEVPNStatus

The possible states of a VPN connection.

