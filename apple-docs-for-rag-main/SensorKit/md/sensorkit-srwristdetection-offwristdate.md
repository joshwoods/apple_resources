

- SensorKit
- SRWristDetection
-  offWristDate 

Instance Property

# offWristDate

The date and time that the user takes their Apple Watch off their wrist.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var offWristDate: Date? { get }
```

## Discussion

Use this property to compute the duration that the user wears their Apple Watch.

The initial value of the offWristDate property is the current date and the onWristDate property is nil. The system changes the value of these properties as follows:

- When the user puts on their Apple Watch, the onWristDate property becomes the current date and the offWristDate property remains the same.

- When the user takes off their Apple Watch, the offWristDate property becomes the current date, and the onWristDate property remains the same.

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

var wristLocation: SRWristDetection.WristLocation

A value that indicates the wrist where the user wears the watch.

enum WristLocation

Preferences for where a user wears a watch.

