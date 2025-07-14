

- AppKit
- NSWindow
-  allowsConcurrentViewDrawing 

Instance Property

# allowsConcurrentViewDrawing

A Boolean value that indicates whether the window allows multithreaded view drawing.

macOS 10.6+

``` source
@MainActor
var allowsConcurrentViewDrawing: Bool { get set }
```

## Discussion

The value of this property is true if the window allows multithreaded view drawing; otherwise, false. The default value is true.

## See Also

### Drawing Windows

func display()

Passes a display message down the window’s view hierarchy, thus redrawing all views within the window.

func displayIfNeeded()

Passes a display message down the window’s view hierarchy, thus redrawing all views that need displaying.

var viewsNeedDisplay: Bool

A Boolean value that indicates whether any of the window’s views need to be displayed.

