

- Core Media
- CMBufferQueue
-  bufferCount 

Instance Property

# bufferCount

The count of buffers in the queue.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var bufferCount: CMItemCount { get }
```

## See Also

### Inspecting a Queue

var isEmpty: Bool

A Boolean value that indicates whether the queue contains buffers.

var head: CMBuffer?

The element at the head of the queue.

var containsEndOfData: Bool

A Boolean value that indicates whether the buffer has its end-of-data state set.

var isAtEndOfData: Bool

A Boolean value that indicates whether that queue is at the end of its data.

