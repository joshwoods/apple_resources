

- AppKit
- NSWindow
-  isModalPanel 

Instance Property

# isModalPanel

A Boolean value that indicates whether the window is a modal panel.

macOS

``` source
@MainActor
var isModalPanel: Bool { get }
```

## Discussion

This property is key-value coding compliant.

## See Also

### Getting Information About Scripting Attributes

var hasCloseBox: Bool

A Boolean value that indicates if the window has a close box.

var hasTitleBar: Bool

A Boolean value that indicates if the window has a title bar.

var isFloatingPanel: Bool

A Boolean value that indicates whether the window is a floating panel.

var isZoomable: Bool

A Boolean value that indicates whether the window allows zooming.

var isResizable: Bool

A Boolean value that indicates if the user can resize the window.

var isMiniaturizable: Bool

A Boolean value that indicates whether the window can minimize.

var orderedIndex: Int

The zero-based position of the window, based on its order from front to back among all visible application windows.

