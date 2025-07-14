

- Network Extension
- NEVPNProtocol
-  disconnectOnSleep 

Instance Property

# disconnectOnSleep

A Boolean value that indicates whether the VPN disconnects when the device sleeps.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var disconnectOnSleep: Bool { get set }
```

## Discussion

The default value of this property is false.

## See Also

### Configuring the VPN

var serverAddress: String?

The address of the VPN server.

var proxySettings: NEProxySettings?

The proxy settings to use for HTTP and HTTPS connections that route through the VPN.

