

- AVFoundation
- AVPlayerItemSegment
-  AVPlayerItemSegment.SegmentType 

Enumeration

# AVPlayerItemSegment.SegmentType

Constants that specify the type of segment.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum SegmentType
```

## Topics

### Segment types

case primary

A segment that represents playback of a primary item.

case interstitial

A segment that represents playback of an interstitial event.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying the type

var segmentType: AVPlayerItemSegment.SegmentType

The type content this segment represents.

