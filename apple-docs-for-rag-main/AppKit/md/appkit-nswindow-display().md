

- AppKit
- NSWindow
-  display() 

Instance Method

# display()

Passes a display message down the window’s view hierarchy, thus redrawing all views within the window.

macOS

``` source
@MainActor
func display()
```

## Discussion

You rarely need to invoke this method. `NSWindow` objects normally record which of their views need displaying and display them automatically on each pass through the event loop.

This method includes the frame view that draws the border, title bar, and other peripheral elements.

## See Also

### Drawing Windows

func displayIfNeeded()

Passes a display message down the window’s view hierarchy, thus redrawing all views that need displaying.

var viewsNeedDisplay: Bool

A Boolean value that indicates whether any of the window’s views need to be displayed.

var allowsConcurrentViewDrawing: Bool

A Boolean value that indicates whether the window allows multithreaded view drawing.

