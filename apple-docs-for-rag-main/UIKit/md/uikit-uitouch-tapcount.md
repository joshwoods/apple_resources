

- UIKit
- UITouch
-  tapCount 

Instance Property

# tapCount

The number of times the finger was tapped for this given touch.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tapCount: Int { get }
```

## Discussion

The value of this property is an integer containing the number of taps that occurred for this touch within a predefined period of time. Use this property to evaluate whether the user single-tapped, double-tapped, or even triple-tapped a particular view or window.

## See Also

### Getting touch attributes

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

func azimuthUnitVector(in: UIView?) -> CGVector

Returns a unit vector that points in the direction of the azimuth of the stylus.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

