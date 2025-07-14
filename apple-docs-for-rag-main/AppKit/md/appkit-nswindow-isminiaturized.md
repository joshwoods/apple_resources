

- AppKit
- NSWindow
-  isMiniaturized 

Instance Property

# isMiniaturized

A Boolean value that indicates whether the window is minimized.

macOS

``` source
@MainActor
var isMiniaturized: Bool { get }
```

## Discussion

The value of this property is true if the window is minimized; otherwise, false. A minimized window is removed from the screen and replaced by a image, icon, or button that represents it, called the counterpart.

## See Also

### Minimizing Windows

func performMiniaturize(Any?)

Simulates the user clicking the minimize button by momentarily highlighting the button, then minimizing the window.

func miniaturize(Any?)

Removes the window from the screen list and displays the minimized window in the Dock.

func deminiaturize(Any?)

De-minimizes the window.

var miniwindowImage: NSImage?

The custom miniaturized window image of the window.

var miniwindowTitle: String!

The title displayed in the window’s minimized window.

