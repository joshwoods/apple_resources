

- Network Extension
- NWTCPConnection
-  txtRecord Deprecated

Instance Property

# txtRecord

The TXT record associated with a connected Bonjour service endpoint.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var txtRecord: Data? { get }
```

Deprecated

Use the nw_endpoint_copy_txt_record(_:) function from the Network framework instead.

## Discussion

When the connection is connected to a Bonjour service endpoint, the TXT record associated with the Bonjour service is available via this property.

Important

Note that the value comes from an untrusted network source. Care must be taken when parsing this potentially malicious value.

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

var connectedPath: NWPath?

The network path over which the connection was established.

Deprecated

