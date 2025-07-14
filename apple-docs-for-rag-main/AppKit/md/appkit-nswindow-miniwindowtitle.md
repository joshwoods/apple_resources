

- AppKit
- NSWindow
-  miniwindowTitle 

Instance Property

# miniwindowTitle

The title displayed in the window’s minimized window.

macOS

``` source
@MainActor
var miniwindowTitle: String! { get set }
```

## Discussion

A minimized window’s title usually reflects that of its full-size counterpart, abbreviated to fit if necessary. Although this property allows you to set the minimized window’s title explicitly, changing the full-size `NSWindow` object’s title (through title or setTitleWithRepresentedFilename(_:)) automatically changes the minimized window’s title as well.

## See Also

### Minimizing Windows

var isMiniaturized: Bool

A Boolean value that indicates whether the window is minimized.

func performMiniaturize(Any?)

Simulates the user clicking the minimize button by momentarily highlighting the button, then minimizing the window.

func miniaturize(Any?)

Removes the window from the screen list and displays the minimized window in the Dock.

func deminiaturize(Any?)

De-minimizes the window.

var miniwindowImage: NSImage?

The custom miniaturized window image of the window.

