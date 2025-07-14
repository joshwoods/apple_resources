

- Core Media
- CMBufferQueue
-  isEmpty 

Instance Property

# isEmpty

A Boolean value that indicates whether the queue contains buffers.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isEmpty: Bool { get }
```

## See Also

### Inspecting a Queue

var bufferCount: CMItemCount

The count of buffers in the queue.

var head: CMBuffer?

The element at the head of the queue.

var containsEndOfData: Bool

A Boolean value that indicates whether the buffer has its end-of-data state set.

var isAtEndOfData: Bool

A Boolean value that indicates whether that queue is at the end of its data.

