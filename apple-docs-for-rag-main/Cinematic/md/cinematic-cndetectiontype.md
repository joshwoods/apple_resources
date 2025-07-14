

- Cinematic
-  CNDetectionType 

Enumeration

# CNDetectionType

The type of object detected, such as face, torso, cat, dog and so on.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
enum CNDetectionType
```

## Topics

### Enumeration Cases

case autoFocus

case catBody

case catHead

case custom

case dogBody

case dogHead

case fixedFocus

case humanFace

case humanHead

case humanTorso

case sportsBall

case unknown

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

### Editing

struct CNDetection

A structure that represents a detected subject, face, torso or pet at a particular time.

struct CNDecision

An object that represents a decision to focus on a particular detection, or group of detections, at a particular time.

class CNDetectionTrack

An object representing a series of detections of the same subject over time.

class CNFixedDetectionTrack

An object representing the fixed detection track.

class CNCustomDetectionTrack

An object representing a discrete detection track composed of individual detections.

