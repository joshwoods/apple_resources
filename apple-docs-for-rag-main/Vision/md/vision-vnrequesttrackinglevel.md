

- Vision
-  VNRequestTrackingLevel 

Enumeration

# VNRequestTrackingLevel

An enumeration of tracking priorities.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum VNRequestTrackingLevel
```

## Topics

### Enumeration Cases

case accurate

Tracking level that favors location accuracy over speed.

case fast

Tracking level that favors speed over location accuracy.

### Creating a Tracking Level

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring a Tracking Request

var inputObservation: VNDetectedObjectObservation

The observation object defining a region to track.

var trackingLevel: VNRequestTrackingLevel

A value for specifying whether to prioritize speed or location accuracy.

var isLastFrame: Bool

A Boolean that indicates the last frame in a tracking sequence.

