

- Network Extension
- NEVPNManager
-  connection 

Instance Property

# connection

An NEVPNConnection object that is used to control the VPN tunnel specified by the VPN configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var connection: NEVPNConnection { get }
```

## Discussion

The connection object is used to manually start and stop the VPN tunnel, and introspect the current status of the VPN tunnel. If the VPN configuration does not exist in the Network Extension preferences then the connection’s status is set to `NEVPNStatusInvalid`.

