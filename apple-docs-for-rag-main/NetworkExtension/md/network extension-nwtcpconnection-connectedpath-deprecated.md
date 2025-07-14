

- Network Extension
- NWTCPConnection
-  connectedPath Deprecated

Instance Property

# connectedPath

The network path over which the connection was established.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var connectedPath: NWPath? { get }
```

Deprecated

Use the nw_connection_copy_current_path(_:) function from the Network framework instead.

## Discussion

The caller can query additional properties from the NWPath object for more information. Note that this contains a snapshot of information at the time of connection establishment for this connection only. As a result, some underlying properties might change in time and might not reflect the path for other connections that might be established at different times.

## See Also

### Getting connection properties

var endpoint: NWEndpoint

The destination endpoint with which this connection was created.

Deprecated

var localAddress: NWEndpoint?

The IP address endpoint from which the connection was established.

Deprecated

var remoteAddress: NWEndpoint?

The IP address endpoint to which the connection was established.

Deprecated

var txtRecord: Data?

The TXT record associated with a connected Bonjour service endpoint.

Deprecated

