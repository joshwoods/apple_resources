

- Cinematic
-  CNObjectTracker 

Class

# CNObjectTracker

An object that converts a normalized point or rectangle into a detection track that tracks an object over time.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
class CNObjectTracker
```

## Topics

### Initializers

init(commandQueue: any MTLCommandQueue)

Creates a new detection track builder.

### Instance Methods

func continueTracking(at: CMTime, sourceImage: CVPixelBuffer, sourceDisparity: CVPixelBuffer) -> CNBoundsPrediction?

An object that continues to track an object that you’ve started tracking, and adds a new detection to the detection track you’re building.

func findObject(at: CGPoint, sourceImage: CVPixelBuffer) -> CNBoundsPrediction?

An object that finds the bounds of an object at the given point.

func finishDetectionTrack() -> CNDetectionTrack

Finish constructing the detection track and return it.

func resetDetectionTrack()

Resets the builder to construct a new detection track.

func startTracking(at: CMTime, within: CGRect, sourceImage: CVPixelBuffer, sourceDisparity: CVPixelBuffer) -> Bool

Starts creating a detection track to track an object within the given bounds.

### Type Properties

static var isSupported: Bool

Indicates whether the current device supports object detection and tracking.

## See Also

### Custom Object Tracking

struct CNBoundsPrediction

A structure representing the bounds of the predicted subject.

