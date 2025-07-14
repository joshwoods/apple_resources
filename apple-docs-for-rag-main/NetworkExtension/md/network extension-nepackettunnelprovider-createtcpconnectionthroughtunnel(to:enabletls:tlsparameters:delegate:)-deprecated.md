

- Network Extension
- NEPacketTunnelProvider
-  createTCPConnectionThroughTunnel(to:enableTLS:tlsParameters:delegate:) Deprecated

Instance Method

# createTCPConnectionThroughTunnel(to:enableTLS:tlsParameters:delegate:)

Create a TCP connection through the current tunnel.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func createTCPConnectionThroughTunnel(
    to remoteEndpoint: NWEndpoint,
    enableTLS: Bool,
    tlsParameters TLSParameters: NWTLSParameters?,
    delegate: Any?
) -> NWTCPConnection
```

Deprecated

Pass the Swift virtualInterface property or the ObjectiveC virtualInterface property to the nw_parameters_require_interface(_:_:) function from the Network framework instead.

## Parameters 

`remoteEndpoint`  

The remote endpoint to connect to.

`enableTLS`  

A flag indicating if the TLS protocol should be used to secure the communication over the connection.

`TLSParameters`  

The TLS protocol parameters to use. If `enableTLS` is true and this parameter is nil then the default TLS parameters will be used.

`delegate`  

An optional delegate object that conforms to the NWTCPConnectionAuthenticationDelegate protocol.

## Discussion

Use this method to create a TCP connection to an endpoint inside the private network.

## See Also

### Creating network connections through the tunnel

func createUDPSessionThroughTunnel(to: NWEndpoint, from: NWHostEndpoint?) -> NWUDPSession

Creates a UDP session through the current tunnel.

Deprecated

