

- AppKit
- NSPanGestureRecognizer
-  translation(in:) 

Instance Method

# translation(in:)

The distance traveled by the mouse during the gesture.

macOS 10.10+

``` source
@MainActor
func translation(in view: NSView?) -> NSPoint
```

## Parameters 

`view`  

The view in whose coordinate system the translation of the pan gesture should be computed. The view’s transform is applied to the distance values.

## Return Value

A point whose x and y values correspond to the total distance travelled since the beginning of the gesture.

## Discussion

The x and y values of the returned point report the total translation over time. They are not delta values from the last time that the translation was reported. To determine the starting point of the gesture, subtract the current translation values from the current location of the mouse in the same view.

## See Also

### Related Documentation

func location(in: NSView?) -> NSPoint

Returns the point computed as the location of the gesture.

### Tracking the Location and Velocity of the Gesture

func setTranslation(NSPoint, in: NSView?)

Changes the current translation value of the gesture recognizer.

func velocity(in: NSView?) -> NSPoint

The velocity of the pan, measured in points per second.

