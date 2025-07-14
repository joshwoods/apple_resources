

- Foundation
- URLSessionTask
-  countOfBytesSent 

Instance Property

# countOfBytesSent

The number of bytes that the task has sent to the server in the request body.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var countOfBytesSent: Int64 { get }
```

## Discussion

This byte count includes *only* the length of the request body itself, not the request headers.

To be notified when this value changes, implement the urlSession(_:task:didSendBodyData:totalBytesSent:totalBytesExpectedToSend:) delegate method.

## See Also

### Obtaining task progress

var progress: Progress

A representation of the overall task progress.

var countOfBytesExpectedToReceive: Int64

The number of bytes that the task expects to receive in the response body.

var countOfBytesReceived: Int64

The number of bytes that the task has received from the server in the response body.

var countOfBytesExpectedToSend: Int64

The number of bytes that the task expects to send in the request body.

let NSURLSessionTransferSizeUnknown: Int64

The total size of the transfer cannot be determined.

