

- AppKit
- NSWindow
-  displayIfNeeded() 

Instance Method

# displayIfNeeded()

Passes a display message down the window’s view hierarchy, thus redrawing all views that need displaying.

macOS

``` source
@MainActor
func displayIfNeeded()
```

## Discussion

This method includes the frame view that draws the border, title bar, and other peripheral elements. It’s useful when you want to modify some number of views and then display only the ones that you modified.

You rarely need to invoke this method. `NSWindow` objects normally record which of their views need displaying and display them automatically on each pass through the event loop.

## See Also

### Drawing Windows

func display()

Passes a display message down the window’s view hierarchy, thus redrawing all views within the window.

var viewsNeedDisplay: Bool

A Boolean value that indicates whether any of the window’s views need to be displayed.

var allowsConcurrentViewDrawing: Bool

A Boolean value that indicates whether the window allows multithreaded view drawing.

