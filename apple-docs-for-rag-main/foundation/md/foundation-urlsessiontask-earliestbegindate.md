

- Foundation
- URLSessionTask
-  earliestBeginDate 

Instance Property

# earliestBeginDate

The earliest date at which the network load should begin.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var earliestBeginDate: Date? { get set }
```

## Mentioned in 

Downloading files in the background

## Discussion

For tasks created from background URLSession instances, this property indicates that the network load should not begin any earlier than this date. Setting this property does not guarantee that the load will begin at the specified date, but only that it will not begin sooner. If not specified, no start delay is used.

This property has no effect for tasks created from nonbackground sessions.

## See Also

### Scheduling tasks

var countOfBytesClientExpectsToReceive: Int64

A best-guess upper bound on the number of bytes the client expects to receive.

var countOfBytesClientExpectsToSend: Int64

A best-guess upper bound on the number of bytes the client expects to send.

let NSURLSessionTransferSizeUnknown: Int64

The total size of the transfer cannot be determined.

