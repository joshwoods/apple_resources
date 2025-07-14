

- Foundation
-  URLSessionTaskTransactionMetrics 

Class

# URLSessionTaskTransactionMetrics

An object that encapsualtes the performance metrics collected by the URL Loading System during the execution of a session task.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class URLSessionTaskTransactionMetrics
```

## Overview

Each URLSessionTaskTransactionMetrics object consists of a request and response property, corresponding to the request and response of the corresponding task. It also contains temporal metrics, starting with fetchStartDate and ending with responseEndDate, as well as other characteristics like networkProtocolName and resourceFetchType.

### Understanding temporal metrics

The figure below shows the sequence of events for a URL session task, which correspond to the temporal metrics captured by URLSessionTaskTransactionMetrics.

For all metrics with a start and end date, if an aspect of the task was not completed, then its corresponding end date metric is `nil`. This can happen if name lookup begins, but the operation either times out, fails, or the client cancels the task before the name can be resolved. In this case, the domainLookupEndDate property is `nil`, along with all metrics for aspects that occurred afterwards.

### Measuring tasks using iCloud Private Relay

iCloud Private Relay can change the timing and sequence of events for your tasks by sending requests through a set of privacy proxies. All tasks that use iCloud Private Relay set the isProxyConnection property in their transaction metrics. In this case, the remoteAddress property contains the address of the proxy, and not the origin server.

Tasks to different hosts can reuse the same transport connection, just like how tasks can already share a connection when using HTTP/2. In these cases, a proxied task may not report any secureConnectionStartDate or secureConnectionEndDate.

## Topics

### Accessing request and response

var request: URLRequest

The transaction request.

var response: URLResponse?

The transaction response.

### Accessing temporal metrics

var fetchStartDate: Date?

The time when the task started fetching the resource, from the server or locally.

var domainLookupStartDate: Date?

The time immediately before the task started the name lookup for the resource.

var domainLookupEndDate: Date?

The time after the name lookup was completed.

var connectStartDate: Date?

The time immediately before the task started establishing a TCP connection to the server.

var secureConnectionStartDate: Date?

The time immediately before the task started the TLS security handshake to secure the current connection.

var secureConnectionEndDate: Date?

The time immediately after the security handshake completed.

var connectEndDate: Date?

The time immediately after the task finished establishing the connection to the server.

var requestStartDate: Date?

The time immediately before the task started requesting the resource, regardless of whether it is retrieved from the server or local resources.

var requestEndDate: Date?

The time immediately after the task finished requesting the resource, regardless of whether it was retrieved from the server or local resources.

var responseStartDate: Date?

The time immediately after the task received the first byte of the response from the server or from local resources.

var responseEndDate: Date?

The time immediately after the task received the last byte of the resource.

### Accessing data transfer metrics

var countOfRequestBodyBytesBeforeEncoding: Int64

The size of the upload body data, file, or stream, in bytes.

var countOfRequestBodyBytesSent: Int64

The number of bytes transferred for the request body.

var countOfRequestHeaderBytesSent: Int64

The number of bytes transferred for the request header.

var countOfResponseBodyBytesAfterDecoding: Int64

The size of data delivered to your delegate or completion handler.

var countOfResponseBodyBytesReceived: Int64

The number of bytes transferred for the response body.

var countOfResponseHeaderBytesReceived: Int64

The number of bytes transferred for the response header.

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

var isProxyConnection: Bool

A Boolean value that indicastes whether the task used a proxy connection to fetch the resource.

var isReusedConnection: Bool

A Boolean value that indicates whether the task used a persistent connection to fetch the resource.

var isMultipath: Bool

A Boolean value that indicates whether the connection uses a successfully negotiated multipath protocol.

var resourceFetchType: URLSessionTaskMetrics.ResourceFetchType

A value that indicates whether the resource was loaded, pushed, or retrieved from the local cache.

enum ResourceFetchType

The manner in which a resource is fetched.

var domainResolutionProtocol: URLSessionTaskMetrics.DomainResolutionProtocol

enum DomainResolutionProtocol

### Creating transaction metrics

init()

Creates a transaction metrics instance.

Deprecated

class func new() -> Self

Creates a new transaction metrics instance.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Accessing task metrics

var transactionMetrics: [URLSessionTaskTransactionMetrics]

An array of metrics for each individual request-response transaction made during the execution of the task.

var taskInterval: DateInterval

The time interval between when a task is instantiated and when the task is completed.

var redirectCount: Int

The number of redirects that occurred during the execution of the task.

