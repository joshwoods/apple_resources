

- AppKit
- NSPanGestureRecognizer
-  velocity(in:) 

Instance Method

# velocity(in:)

The velocity of the pan, measured in points per second.

macOS 10.10+

``` source
@MainActor
func velocity(in view: NSView?) -> NSPoint
```

## Parameters 

`view`  

The view that provides the coordinate system for computing the velocity value. This parameter must not be `nil`.

## Return Value

The horizontal and vertical velocity of the pan gesture. These values are relative to the specified view.

## See Also

### Tracking the Location and Velocity of the Gesture

func translation(in: NSView?) -> NSPoint

The distance traveled by the mouse during the gesture.

func setTranslation(NSPoint, in: NSView?)

Changes the current translation value of the gesture recognizer.

