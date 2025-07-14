

- SensorKit
- SRWristDetection
-  SRWristDetection.WristLocation 

Enumeration

# SRWristDetection.WristLocation

Preferences for where a user wears a watch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum WristLocation
```

## Topics

### Wrist Preferences

case left

Indicates that the user wears a watch on the left wrist.

case right

Indicates that the user wears a watch on the right wrist.

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

enum CrownOrientation

Directions the Digital Crown can face with respect to the wearer.

var onWrist: Bool

A value that indicates whether the watch is on the user’s wrist.

var onWristDate: Date?

The date and time that the user puts their Apple Watch on their wrist.

var offWristDate: Date?

The date and time that the user takes their Apple Watch off their wrist.

var wristLocation: SRWristDetection.WristLocation

A value that indicates the wrist where the user wears the watch.

