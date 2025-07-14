

- AppKit
- NSWindow
-  viewsNeedDisplay 

Instance Property

# viewsNeedDisplay

A Boolean value that indicates whether any of the window’s views need to be displayed.

macOS

``` source
@MainActor
var viewsNeedDisplay: Bool { get set }
```

## Discussion

The value of this property is true when any of the window’s views need to be displayed; otherwise, false. You should rarely need to set this property; the `NSView` method needsDisplay and similar methods set it automatically.

## See Also

### Drawing Windows

func display()

Passes a display message down the window’s view hierarchy, thus redrawing all views within the window.

func displayIfNeeded()

Passes a display message down the window’s view hierarchy, thus redrawing all views that need displaying.

var allowsConcurrentViewDrawing: Bool

A Boolean value that indicates whether the window allows multithreaded view drawing.

