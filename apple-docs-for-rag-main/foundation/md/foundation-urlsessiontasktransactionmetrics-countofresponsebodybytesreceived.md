

- Foundation
- URLSessionTaskTransactionMetrics
-  countOfResponseBodyBytesReceived 

Instance Property

# countOfResponseBodyBytesReceived

The number of bytes transferred for the response body.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var countOfResponseBodyBytesReceived: Int64 { get }
```

## Discussion

This value includes protocol-specific framing, transfer encoding, and content encoding.

## See Also

### Accessing data transfer metrics

var countOfRequestBodyBytesBeforeEncoding: Int64

The size of the upload body data, file, or stream, in bytes.

var countOfRequestBodyBytesSent: Int64

The number of bytes transferred for the request body.

var countOfRequestHeaderBytesSent: Int64

The number of bytes transferred for the request header.

var countOfResponseBodyBytesAfterDecoding: Int64

The size of data delivered to your delegate or completion handler.

var countOfResponseHeaderBytesReceived: Int64

The number of bytes transferred for the response header.

