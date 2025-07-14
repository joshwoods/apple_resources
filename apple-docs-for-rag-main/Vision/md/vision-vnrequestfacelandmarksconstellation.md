

- Vision
-  VNRequestFaceLandmarksConstellation 

Enumeration

# VNRequestFaceLandmarksConstellation

An enumeration of face landmarks in a constellation object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum VNRequestFaceLandmarksConstellation
```

## Topics

### Types of Constellations

case constellationNotDefined

An undefined constellation.

case constellation65Points

A constellation with 65 points.

case constellation76Points

A constellation with 76 points.

### Creating a Constellation

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Locating Face Landmarks

var constellation: VNRequestFaceLandmarksConstellation

A variable that describes how a face landmarks request orders or enumerates the resulting features.

