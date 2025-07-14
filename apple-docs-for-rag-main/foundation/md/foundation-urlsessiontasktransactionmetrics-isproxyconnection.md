

- Foundation
- URLSessionTaskTransactionMetrics
-  isProxyConnection 

Instance Property

# isProxyConnection

A Boolean value that indicastes whether the task used a proxy connection to fetch the resource.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var isProxyConnection: Bool { get }
```

## See Also

### Accessing transaction characteristics

var networkProtocolName: String?

The network protocol used to fetch the resource.

var remoteAddress: String?

The IP address string of the remote interface for the connection.

var remotePort: Int?

The port number of the remote interface for the connection.

var localAddress: String?

The IP address string of the local interface for the connection.

var localPort: Int?

The port number of the local interface for the connection.

var negotiatedTLSCipherSuite: tls_ciphersuite_t?

The TLS cipher suite the task negotiated with the endpoint for the connection.

var negotiatedTLSProtocolVersion: tls_protocol_version_t?

The TLS protocol version the task negotiated with the endpoint for the connection.

var isCellular: Bool

A Boolean value that indicates whether the connection operates over a cellular interface.

var isExpensive: Bool

A Boolean value that indicates whether the connection operates over an expensive interface.

var isConstrained: Bool

A Boolean value that indicates whether the connection operates over an interface marked as constrained.

var isReusedConnection: Bool

A Boolean value that indicates whether the task used a persistent connection to fetch the resource.

var isMultipath: Bool

A Boolean value that indicates whether the connection uses a successfully negotiated multipath protocol.

var resourceFetchType: URLSessionTaskMetrics.ResourceFetchType

A value that indicates whether the resource was loaded, pushed, or retrieved from the local cache.

enum ResourceFetchType

The manner in which a resource is fetched.

var domainResolutionProtocol: URLSessionTaskMetrics.DomainResolutionProtocol

