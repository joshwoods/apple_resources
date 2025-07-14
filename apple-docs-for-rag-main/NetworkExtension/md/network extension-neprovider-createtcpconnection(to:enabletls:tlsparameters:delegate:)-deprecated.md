

- Network Extension
- NEProvider
-  createTCPConnection(to:enableTLS:tlsParameters:delegate:) Deprecated

Instance Method

# createTCPConnection(to:enableTLS:tlsParameters:delegate:)

Create a TCP connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func createTCPConnection(
    to remoteEndpoint: NWEndpoint,
    enableTLS: Bool,
    tlsParameters TLSParameters: NWTLSParameters?,
    delegate: Any?
) -> NWTCPConnection
```

Deprecated

Use the nw_connection_t type from the Network framework instead.

## Parameters 

`remoteEndpoint`  

The remote endpoint to connect to.

`enableTLS`  

A flag indicating if the TLS protocol should be used to secure the communication over the connection.

`TLSParameters`  

The TLS protocol parameters to use. If `enableTLS` is true and this parameter is nil then the default TLS parameters will be used.

`delegate`  

An optional delegate object that conforms to the NWTCPConnectionAuthenticationDelegate protocol.

## Return Value

A NWTCPConnection object. The underlying connection is in the process of being established. You can observe the connection’s `state` property using KVO to determine when the connection is successfully established or fails due to an error. For information about KVO, see Key-Value Observing Programming Guide.

## Discussion

This method provides a convenient way to create TCP connections from a Network Extension Provider. It is preferred over using the sockets API. For instance, the Tunnel Provider can use this method to create a secure TCP connection with the tunnel server that can be used to tunnel network data.

## See Also

### Creating network connections

func createUDPSession(to: NWEndpoint, from: NWHostEndpoint?) -> NWUDPSession

Creates a UDP session.

Deprecated

