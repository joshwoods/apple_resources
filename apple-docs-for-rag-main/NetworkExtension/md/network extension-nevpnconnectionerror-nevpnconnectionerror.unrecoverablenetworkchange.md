

- Network Extension
- NEVPNConnectionError
-  NEVPNConnectionError.unrecoverableNetworkChange 

Case

# NEVPNConnectionError.unrecoverableNetworkChange

An error code that indicates network conditions changed such that the VPN connection needed to terminate.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
case unrecoverableNetworkChange
```

## See Also

### General error codes

case overslept

An error code that indicates the system slept for an extended period of time, causing the VPN connection to terminate.

case noNetworkAvailable

An error code that indicates the VPN connection failed because the system isn’t connected to a network.

case configurationFailed

An error code that indicates the VPN connection failed because the configuration is invalid.

case authenticationFailed

An error code that indicates the VPN connection failed because the VPN server rejected the user credentials.

case configurationNotFound

An error code that indicates the VPN connection failed because the system couldn’t find a configuration.

case negotiationFailed

An error code that indicates the VPN connection failed because the negotiation failed.

