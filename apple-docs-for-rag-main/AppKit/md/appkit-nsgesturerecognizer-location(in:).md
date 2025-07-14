

- AppKit
- NSGestureRecognizer
-  location(in:) 

Instance Method

# location(in:)

Returns the point computed as the location of the gesture.

macOS 10.10+

``` source
@MainActor
func location(in view: NSView?) -> NSPoint
```

## Parameters 

`view`  

The view whose coordinate system you want to use for determining the location of the gesture. Specify `nil` to return the point in the coordinate system of the window.

## Return Value

The point at which the gesture occurred. The returned point is in the coordinate system of the specified view, or in the coordinate system of the window if you specified `nil` for the view parameter.

## Discussion

Use this method to determine the location at which the gesture occurred. Subclasses are responsible for overriding this method and returning an appropriate value based on the type of gesture.

For specific information about what the returned point represents, see the specific gesture recognizer subclass.

