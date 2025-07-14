

- Core Media
-  CMBuffer 

Type Alias

# CMBuffer

A reference to a buffer object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBuffer = CFTypeRef
```

## Discussion

A `CMBuffer` can be an instance of any Core Foundation type, as long as a `getDuration` callback can be provided. Commonly used types are `CMSampleBuffer` and `CVPixelBuffer`.

## See Also

### Data Types

class CMSampleBuffer

A reference to a buffer of media data.

Sample Buffer Flags

Flags that customize the behavior of framework operations.

struct CMSampleTimingInfo

A collection of timing information for a sample in a sample buffer.

typealias CMBufferGetSizeCallback

A client callback that returns a size.

typealias CMItemIndex

A datatype that represents an item index.

typealias CMItemCount

A datatype that represents an item count.

typealias CMPersistentTrackID

A datatype that represents a persistent track identifier.

typealias CMMuxedStreamType

A datatype that represents a muxed stream of data.

