

- Cinematic
-  CNDetectionTrack 

Class

# CNDetectionTrack

An object representing a series of detections of the same subject over time.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
class CNDetectionTrack
```

## Topics

### Instance Properties

var detectionGroupID: CNDetectionGroupID

The detection group ID of the subject detected by the track.

var detectionID: CNDetectionID

The unique ID of the subject detected during this track.

var detectionType: CNDetectionType

The type of object that’s detected.

var isDiscrete: Bool

A flag determining if the detection track has discrete detections, otherwise continuous.

var isUserCreated: Bool

A flag indicating if the client created the detection track.

### Instance Methods

func detection(atOrBefore: CMTime) -> CNDetection?

Returns the array of detections in the detection track before a given time.

func detection(nearest: CMTime) -> CNDetection?

Returns the array of detections in the detection track nearest a given time.

func detections(in: CMTimeRange) -> [CNDetection]

Returns the array of detections in the detection track within the given time range.

## Relationships

### Inherited By

- CNCustomDetectionTrack
- CNFixedDetectionTrack

## See Also

### Editing

struct CNDetection

A structure that represents a detected subject, face, torso or pet at a particular time.

struct CNDecision

An object that represents a decision to focus on a particular detection, or group of detections, at a particular time.

class CNFixedDetectionTrack

An object representing the fixed detection track.

class CNCustomDetectionTrack

An object representing a discrete detection track composed of individual detections.

enum CNDetectionType

The type of object detected, such as face, torso, cat, dog and so on.

