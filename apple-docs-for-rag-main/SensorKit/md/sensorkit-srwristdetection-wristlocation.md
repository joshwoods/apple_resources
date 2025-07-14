

- SensorKit
- SRWristDetection
-  wristLocation 

Instance Property

# wristLocation

A value that indicates the wrist where the user wears the watch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var wristLocation: SRWristDetection.WristLocation { get }
```

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

enum WristLocation

Preferences for where a user wears a watch.

