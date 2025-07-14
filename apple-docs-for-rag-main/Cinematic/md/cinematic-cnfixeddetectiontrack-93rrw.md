

- Cinematic
-  CNFixedDetectionTrack 

Class

# CNFixedDetectionTrack

An object representing the fixed detection track.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
class CNFixedDetectionTrack
```

## Topics

### Initializers

init(focusDisparity: Float)

Creates a detection track with fixed focus at the given disparity.

init(originalDetection: CNDetection)

Creates a detection track with fixed focus at the disparity of an existing detection.

### Instance Properties

var focusDisparity: Float

The disparity to use in order to focus on the object.

var originalDetection: CNDetection?

The original detection based on the fixed detection track.

## Relationships

### Inherits From

- CNDetectionTrack

## See Also

### Editing

struct CNDetection

A structure that represents a detected subject, face, torso or pet at a particular time.

struct CNDecision

An object that represents a decision to focus on a particular detection, or group of detections, at a particular time.

class CNDetectionTrack

An object representing a series of detections of the same subject over time.

class CNCustomDetectionTrack

An object representing a discrete detection track composed of individual detections.

enum CNDetectionType

The type of object detected, such as face, torso, cat, dog and so on.

