

- Foundation
- URLSessionTask
-  countOfBytesClientExpectsToReceive 

Instance Property

# countOfBytesClientExpectsToReceive

A best-guess upper bound on the number of bytes the client expects to receive.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var countOfBytesClientExpectsToReceive: Int64 { get set }
```

## Mentioned in 

Downloading files in the background

## Discussion

The value set for this property should account for the size of both HTTP response headers and the response body. If no value is specified, the system uses NSURLSessionTransferSizeUnknown instead. This property is used by the system to optimize the scheduling of URL session tasks. Developers are strongly encouraged to provide an approximate upper bound, or an exact byte count, if possible, rather than accept the default.

## See Also

### Scheduling tasks

var countOfBytesClientExpectsToSend: Int64

A best-guess upper bound on the number of bytes the client expects to send.

let NSURLSessionTransferSizeUnknown: Int64

The total size of the transfer cannot be determined.

var earliestBeginDate: Date?

The earliest date at which the network load should begin.

