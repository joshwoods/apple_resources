

- Core Media
-  CMBufferGetSizeCallback 

Type Alias

# CMBufferGetSizeCallback

A client callback that returns a size.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBufferGetSizeCallback = (CMBuffer, UnsafeMutableRawPointer?) -> Int
```

## Parameters 

`buf`  

The buffer being interrogated.

`refcon`  

The client refcon. Can be `NULL`.

## See Also

### Data Types

class CMSampleBuffer

A reference to a buffer of media data.

Sample Buffer Flags

Flags that customize the behavior of framework operations.

struct CMSampleTimingInfo

A collection of timing information for a sample in a sample buffer.

typealias CMBuffer

A reference to a buffer object.

typealias CMItemIndex

A datatype that represents an item index.

typealias CMItemCount

A datatype that represents an item count.

typealias CMPersistentTrackID

A datatype that represents a persistent track identifier.

typealias CMMuxedStreamType

A datatype that represents a muxed stream of data.

