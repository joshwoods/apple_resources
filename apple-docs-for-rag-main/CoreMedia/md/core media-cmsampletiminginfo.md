

- Core Media
-  CMSampleTimingInfo 

Structure

# CMSampleTimingInfo

A collection of timing information for a sample in a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMSampleTimingInfo
```

## Overview

A single `CMSampleTimingInfo` struct can describe every individual sample in a `CMSampleBuffer`, if the samples all have the same duration and are in presentation order with no gaps.

## Topics

### Constants

static let invalid: CMSampleTimingInfo

### Initializers

init()

init(duration: CMTime, presentationTimeStamp: CMTime, decodeTimeStamp: CMTime)

### Properties

var decodeTimeStamp: CMTime

The time at which the sample will be decoded.

var duration: CMTime

The duration of the sample.

var presentationTimeStamp: CMTime

The time at which the sample will be presented.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

class CMSampleBuffer

A reference to a buffer of media data.

Sample Buffer Flags

Flags that customize the behavior of framework operations.

typealias CMBuffer

A reference to a buffer object.

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

