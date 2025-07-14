

- UIKit
- UITouch
-  maximumPossibleForce 

Instance Property

# maximumPossibleForce

The maximum possible force for a touch.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var maximumPossibleForce: CGFloat { get }
```

## Discussion

The value of this property is sufficiently high to provide a wide dynamic range for values of the force property.

This property is available on devices that support 3D Touch or Apple Pencil. To check at runtime if a device supports 3D Touch, read the value of the forceTouchCapability property on the trait collection for any object in your app with a trait environment.

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

var altitudeAngle: CGFloat

The altitude (in radians) of the stylus.

func azimuthAngle(in: UIView?) -> CGFloat

Returns the azimuth angle (in radians) of the stylus.

func azimuthUnitVector(in: UIView?) -> CGVector

Returns a unit vector that points in the direction of the azimuth of the stylus.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

