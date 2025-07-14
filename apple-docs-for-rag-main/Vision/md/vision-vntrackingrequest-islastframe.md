

- Vision
- VNTrackingRequest
-  isLastFrame 

Instance Property

# isLastFrame

A Boolean that indicates the last frame in a tracking sequence.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var isLastFrame: Bool { get set }
```

## Discussion

If set to true, the current tracker will be released to the pool of available trackers when the current frame finishes processing.

## See Also

### Configuring a Tracking Request

enum VNRequestTrackingLevel

An enumeration of tracking priorities.

var inputObservation: VNDetectedObjectObservation

The observation object defining a region to track.

var trackingLevel: VNRequestTrackingLevel

A value for specifying whether to prioritize speed or location accuracy.

