

- UIKit
- UITouch
-  azimuthAngle(in:) 

Instance Method

# azimuthAngle(in:)

Returns the azimuth angle (in radians) of the stylus.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func azimuthAngle(in view: UIView?) -> CGFloat
```

## Parameters 

`view`  

The view that contains the stylus’s touch. Pass `nil` to get the azimuth angle that is relative to the touch’s window.

## Return Value

The azimuth angle of the stylus, in radians.

## Discussion

In the plane of the screen, the azimuth angle is the direction in which the stylus is pointing. With the tip of the stylus touching the screen, the value of this property is `0` radians when the cap end of the stylus (that is, the end opposite of the tip) points along the positive x axis of the device’s screen. The azimuth angle increases as the user swings the cap end of the stylus in a clockwise direction around the tip.

Note

It is more expensive to get the azimuth angle (as opposed to the azimuth unit vector), but it can also be more convenient

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

func azimuthUnitVector(in: UIView?) -> CGVector

Returns a unit vector that points in the direction of the azimuth of the stylus.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

