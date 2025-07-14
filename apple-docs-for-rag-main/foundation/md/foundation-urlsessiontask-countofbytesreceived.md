

- Foundation
- URLSessionTask
-  countOfBytesReceived 

Instance Property

# countOfBytesReceived

The number of bytes that the task has received from the server in the response body.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var countOfBytesReceived: Int64 { get }
```

## Discussion

To be notified when this value changes, implement the urlSession(_:dataTask:didReceive:) delegate method (for data and upload tasks) or the urlSession(_:downloadTask:didWriteData:totalBytesWritten:totalBytesExpectedToWrite:) method (for download tasks).

## See Also

### Obtaining task progress

var progress: Progress

A representation of the overall task progress.

var countOfBytesExpectedToReceive: Int64

The number of bytes that the task expects to receive in the response body.

var countOfBytesExpectedToSend: Int64

The number of bytes that the task expects to send in the request body.

var countOfBytesSent: Int64

The number of bytes that the task has sent to the server in the request body.

let NSURLSessionTransferSizeUnknown: Int64

The total size of the transfer cannot be determined.

