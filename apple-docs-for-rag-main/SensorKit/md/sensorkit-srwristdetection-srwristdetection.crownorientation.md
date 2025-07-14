

- SensorKit
- SRWristDetection
-  SRWristDetection.CrownOrientation 

Enumeration

# SRWristDetection.CrownOrientation

Directions the Digital Crown can face with respect to the wearer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum CrownOrientation
```

## Topics

### Orientations

case left

Indicates that the Digital Crown faces to the left with respect to the wearer.

case right

Indicates that the Digital Crown faces to the right with respect to the wearer.

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

### Inspecting Watch Configuration

var crownOrientation: SRWristDetection.CrownOrientation

A value that indicates the direction the Digital Crown faces with respect to the user.

var onWrist: Bool

A value that indicates whether the watch is on the user’s wrist.

var onWristDate: Date?

The date and time that the user puts their Apple Watch on their wrist.

var offWristDate: Date?

The date and time that the user takes their Apple Watch off their wrist.

var wristLocation: SRWristDetection.WristLocation

A value that indicates the wrist where the user wears the watch.

enum WristLocation

Preferences for where a user wears a watch.

