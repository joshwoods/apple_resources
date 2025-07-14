

- Foundation
- URLSessionTaskTransactionMetrics
-  connectEndDate 

Instance Property

# connectEndDate

The time immediately after the task finished establishing the connection to the server.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var connectEndDate: Date? { get }
```

## Discussion

This value accounts for completion of security-related and other handshakes. The value will be `nil` if a persistent connection is used, or if the resource is retrieved from local resources.

## See Also

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

var requestStartDate: Date?

The time immediately before the task started requesting the resource, regardless of whether it is retrieved from the server or local resources.

var requestEndDate: Date?

The time immediately after the task finished requesting the resource, regardless of whether it was retrieved from the server or local resources.

var responseStartDate: Date?

The time immediately after the task received the first byte of the response from the server or from local resources.

var responseEndDate: Date?

The time immediately after the task received the last byte of the resource.

