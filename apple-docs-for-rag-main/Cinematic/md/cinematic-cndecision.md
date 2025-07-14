

- Cinematic
-  CNDecision 

Structure

# CNDecision

An object that represents a decision to focus on a particular detection, or group of detections, at a particular time.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
struct CNDecision
```

## Topics

### Initializers

init(time: CMTime, detectionGroupID: CNDetectionGroupID, strong: Bool)

Makes a decision to focus on the detection with the given unique detection.

init(time: CMTime, detectionID: CNDetectionID, strong: Bool)

Makes a decision to focus on the best among those detections with the same detection group ID.

### Instance Properties

var focusDetectionID: CNDecision.FocusDetectionID

var isStrongDecision: Bool

A flag representing whether this is a strong decision.

var isUserDecision: Bool

A flag representing whether this is a user-created decision or a base decision.

var time: CMTime

The first presentation time that the subject should be in focus.

### Enumerations

enum FocusDetectionID

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Editing

struct CNDetection

A structure that represents a detected subject, face, torso or pet at a particular time.

class CNDetectionTrack

An object representing a series of detections of the same subject over time.

class CNFixedDetectionTrack

An object representing the fixed detection track.

class CNCustomDetectionTrack

An object representing a discrete detection track composed of individual detections.

enum CNDetectionType

The type of object detected, such as face, torso, cat, dog and so on.

