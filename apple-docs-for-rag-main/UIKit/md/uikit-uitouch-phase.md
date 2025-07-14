

- UIKit
- UITouch
-  phase 

Instance Property

# phase

The phase of the touch.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var phase: UITouch.Phase { get }
```

## Discussion

The property value is a constant that indicates whether the touch began, moved, ended, or was canceled. For descriptions of the possible values of this property, see UITouch.Phase.

## See Also

### Getting touch attributes

var tapCount: Int

The number of times the finger was tapped for this given touch.

var timestamp: TimeInterval

The time when the touch occurred or when it was last mutated.

var type: UITouch.TouchType

The type of the touch.

enum TouchType

The type of touch received.

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

