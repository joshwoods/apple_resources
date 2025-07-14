

- AppKit
- NSMediaLibraryBrowserController
-  isVisible 

Instance Property

# isVisible

A Boolean value that determines whether the Media Library Browser panel is visible.

macOS 10.9+

``` source
var isVisible: Bool { get set }
```

## Discussion

Set this value to true to show the Media Library Browser or false to hide it.

This value can be read to determine the current visibility status of the panel.

## See Also

### Displaying the Media Library Browser Panel

var frame: NSRect

The frame, in global coordinates, used to display the Media Library Browser panel.

func togglePanel(Any?)

Toggles the visibility of the Media Library Browser.

