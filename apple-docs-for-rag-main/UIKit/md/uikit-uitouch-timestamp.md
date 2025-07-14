

- UIKit
- UITouch
-  timestamp 

Instance Property

# timestamp

The time when the touch occurred or when it was last mutated.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var timestamp: TimeInterval { get }
```

## Discussion

The value of this property is the time, in seconds since system startup, that the touch originated or was last changed. You can store the value of this property and compare it to the timestamp in subsequent UITouch objects to determine the duration of the touch and, if it is being swiped, the speed of movement. For a definition of the time since system startup, see the description of the systemUptime method of the ProcessInfo class.

## See Also

### Getting touch attributes

var tapCount: Int

The number of times the finger was tapped for this given touch.

var type: UITouch.TouchType

The type of the touch.

enum TouchType

The type of touch received.

var phase: UITouch.Phase

The phase of the touch.

enum Phase

The phase of a touch event.

var force: CGFloat

The force of the touch, where a value of `1.0` represents the force of an average touch (predetermined by the system, not user-specific).

var maximumPossibleForce: CGFloat

The maximum possible force for a touch.

var altitudeAngle: CGFloat

The altitude (in radians) of the stylus.

func azimuthAngle(in: UIView?) -> CGFloat

Returns the azimuth angle (in radians) of the stylus.

func azimuthUnitVector(in: UIView?) -> CGVector

Returns a unit vector that points in the direction of the azimuth of the stylus.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

