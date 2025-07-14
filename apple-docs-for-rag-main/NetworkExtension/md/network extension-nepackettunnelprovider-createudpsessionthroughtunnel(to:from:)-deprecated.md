

- Network Extension
- NEPacketTunnelProvider
-  createUDPSessionThroughTunnel(to:from:) Deprecated

Instance Method

# createUDPSessionThroughTunnel(to:from:)

Creates a UDP session through the current tunnel.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func createUDPSessionThroughTunnel(
    to remoteEndpoint: NWEndpoint,
    from localEndpoint: NWHostEndpoint?
) -> NWUDPSession
```

Deprecated

Pass the Swift virtualInterface property or the ObjectiveC virtualInterface property to the nw_parameters_require_interface(_:_:) function from the Network framework instead.

## Parameters 

`remoteEndpoint`  

The remote endpoint to send UDP datagrams to.

`localEndpoint`  

The local endpoint to bind the UDP session to. If nil, the UDP session will be bound to an ephemeral port on the virtual interface.

## Discussion

Use this method to create a UDP session to an endpoint inside the private network.

## See Also

### Creating network connections through the tunnel

func createTCPConnectionThroughTunnel(to: NWEndpoint, enableTLS: Bool, tlsParameters: NWTLSParameters?, delegate: Any?) -> NWTCPConnection

Create a TCP connection through the current tunnel.

Deprecated

