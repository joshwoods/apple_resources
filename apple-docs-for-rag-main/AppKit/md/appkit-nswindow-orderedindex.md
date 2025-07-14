

- AppKit
- NSWindow
-  orderedIndex 

Instance Property

# orderedIndex

The zero-based position of the window, based on its order from front to back among all visible application windows.

macOS

``` source
@MainActor
var orderedIndex: Int { get set }
```

## Discussion

If you set this property to an index that’s out of range, the system sets the position to the nearest value that’s in range.

## See Also

### Getting Information About Scripting Attributes

var hasCloseBox: Bool

A Boolean value that indicates if the window has a close box.

var hasTitleBar: Bool

A Boolean value that indicates if the window has a title bar.

var isModalPanel: Bool

A Boolean value that indicates whether the window is a modal panel.

var isFloatingPanel: Bool

A Boolean value that indicates whether the window is a floating panel.

var isZoomable: Bool

A Boolean value that indicates whether the window allows zooming.

var isResizable: Bool

A Boolean value that indicates if the user can resize the window.

var isMiniaturizable: Bool

A Boolean value that indicates whether the window can minimize.

