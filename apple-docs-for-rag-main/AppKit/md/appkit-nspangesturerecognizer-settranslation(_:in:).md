

- AppKit
- NSPanGestureRecognizer
-  setTranslation(\_:in:) 

Instance Method

# setTranslation(\_:in:)

Changes the current translation value of the gesture recognizer.

macOS 10.10+

``` source
@MainActor
func setTranslation(
    _ translation: NSPoint,
    in view: NSView?
)
```

## Parameters 

`translation`  

The new translation values to use in the gesture recognizer.

`view`  

The view in whose coordinate system you specified the new translation value. Specifying `nil` resets the previous translation value.

## Discussion

This method changes the current translation value of the gesture recognizer. Changing the value resets the velocity of the pan. You might call this method at mouse-down time to adjust the translation value and make it relative to some specific point in your view.

## See Also

### Tracking the Location and Velocity of the Gesture

func translation(in: NSView?) -> NSPoint

The distance traveled by the mouse during the gesture.

func velocity(in: NSView?) -> NSPoint

The velocity of the pan, measured in points per second.

