

- UIKit
- UITouch
-  azimuthUnitVector(in:) 

Instance Method

# azimuthUnitVector(in:)

Returns a unit vector that points in the direction of the azimuth of the stylus.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func azimuthUnitVector(in view: UIView?) -> CGVector
```

## Parameters 

`view`  

The view that contains the stylus’s touch. Pass `nil` to get the unit vector for the azimuth that is relative to the touch’s window.

## Return Value

The unit vector that points in the direction of the azimuth of the stylus.

## Discussion

It is less expensive to get the azimuth unit vector than the azimuth angle. If you’re creating transform matrices, the unit vector can also be more useful.

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

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

