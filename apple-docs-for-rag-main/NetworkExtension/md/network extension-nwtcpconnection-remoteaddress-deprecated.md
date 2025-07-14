

- Network Extension
- NWTCPConnection
-  remoteAddress Deprecated

Instance Property

# remoteAddress

The IP address endpoint to which the connection was established.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var remoteAddress: NWEndpoint? { get }
```

Deprecated

Use the nw_path_copy_effective_remote_endpoint(_:) function from the Network framework instead.

## See Also

### Getting connection properties

var endpoint: NWEndpoint

The destination endpoint with which this connection was created.

Deprecated

var localAddress: NWEndpoint?

The IP address endpoint from which the connection was established.

Deprecated

var connectedPath: NWPath?

The network path over which the connection was established.

Deprecated

var txtRecord: Data?

The TXT record associated with a connected Bonjour service endpoint.

Deprecated

