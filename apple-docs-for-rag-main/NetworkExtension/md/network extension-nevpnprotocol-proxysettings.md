

- Network Extension
- NEVPNProtocol
-  proxySettings 

Instance Property

# proxySettings

The proxy settings to use for HTTP and HTTPS connections that route through the VPN.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var proxySettings: NEProxySettings? { get set }
```

## Discussion

While operating under an established VPN tunnel, HTTP and HTTPS connections inside the tunnel use the given proxy settings.

## See Also

### Configuring the VPN

var serverAddress: String?

The address of the VPN server.

var disconnectOnSleep: Bool

A Boolean value that indicates whether the VPN disconnects when the device sleeps.

