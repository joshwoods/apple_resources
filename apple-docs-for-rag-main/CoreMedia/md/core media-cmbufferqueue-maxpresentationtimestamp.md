

- Core Media
- CMBufferQueue
-  maxPresentationTimeStamp 

Instance Property

# maxPresentationTimeStamp

The greatest presentation timestamp.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var maxPresentationTimeStamp: CMTime { get }
```

## See Also

### Inspecting Duration and Timing

var duration: CMTime

The sum of all durations of buffers in the queue.

var totalSize: Int

The total size of all buffers in the queue.

var firstDecodeTimeStamp: CMTime

The decode timestamp of the first buffer in the queue.

var firstPresentationTimeStamp: CMTime

The presentation timestamp of the first buffer in the queue.

var endPresentationTimeStamp: CMTime

The greatest end presentation timestamp.

var minDecodeTimeStamp: CMTime

The earliest decode timestamp.

var minPresentationTimeStamp: CMTime

The earliest presentation timestamp.

