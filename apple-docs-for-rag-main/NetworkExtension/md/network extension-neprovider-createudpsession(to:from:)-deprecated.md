

- Network Extension
- NEProvider
-  createUDPSession(to:from:) Deprecated

Instance Method

# createUDPSession(to:from:)

Creates a UDP session.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func createUDPSession(
    to remoteEndpoint: NWEndpoint,
    from localEndpoint: NWHostEndpoint?
) -> NWUDPSession
```

Deprecated

Use the nw_connection_t type from the Network framework instead.

## Parameters 

`remoteEndpoint`  

The remote endpoint to send UDP datagrams to.

`localEndpoint`  

The local endpoint to bind the UDP session to. If nil, the UDP session will be bound to an ephemeral port on the primary physical interface.

## Return Value

A NWUDPSession object. The remote endpoint is in the process of being resolved. You can observe the session’s `state` property using KVO to determine when the session can be used to send and receive UDP datagrams.

## Discussion

This method provides a convenient way to create UDP connections from a Network Extension Provider. It is preferred over using the sockets API. For instance, the Tunnel Provider can use this method to create a UDP connection with the tunnel server that can be used to tunnel network data.

## See Also

### Creating network connections

func createTCPConnection(to: NWEndpoint, enableTLS: Bool, tlsParameters: NWTLSParameters?, delegate: Any?) -> NWTCPConnection

Create a TCP connection.

Deprecated

