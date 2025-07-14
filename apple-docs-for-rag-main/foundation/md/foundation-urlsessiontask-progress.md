

- Foundation
- URLSessionTask
-  progress 

Instance Property

# progress

A representation of the overall task progress.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var progress: Progress { get }
```

## Mentioned in 

Downloading files from websites

## See Also

### Obtaining task progress

var countOfBytesExpectedToReceive: Int64

The number of bytes that the task expects to receive in the response body.

var countOfBytesReceived: Int64

The number of bytes that the task has received from the server in the response body.

var countOfBytesExpectedToSend: Int64

The number of bytes that the task expects to send in the request body.

var countOfBytesSent: Int64

The number of bytes that the task has sent to the server in the request body.

let NSURLSessionTransferSizeUnknown: Int64

The total size of the transfer cannot be determined.

