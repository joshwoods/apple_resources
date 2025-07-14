

- Core Media
- CMBufferQueue
-  isAtEndOfData 

Instance Property

# isAtEndOfData

A Boolean value that indicates whether that queue is at the end of its data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isAtEndOfData: Bool { get }
```

## See Also

### Inspecting a Queue

var isEmpty: Bool

A Boolean value that indicates whether the queue contains buffers.

var bufferCount: CMItemCount

The count of buffers in the queue.

var head: CMBuffer?

The element at the head of the queue.

var containsEndOfData: Bool

A Boolean value that indicates whether the buffer has its end-of-data state set.

