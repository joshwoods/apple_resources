

- AppKit
- NSWindow
-  canBecomeMain 

Instance Property

# canBecomeMain

A Boolean value that indicates whether the window can become the application’s main window.

macOS

``` source
@MainActor
var canBecomeMain: Bool { get }
```

## Discussion

The value of this property is true when the window can become the main window; otherwise, false.

Attempts to make the window the main window are abandoned if the value of this property is false. The value of the property is true if the window is visible, is not an NSPanel object, and has a title bar or a resize mechanism. Otherwise, the value is false.

## See Also

### Managing Main Status

var isMainWindow: Bool

A Boolean value that indicates whether the window is the application’s main window.

func makeMain()

Makes the window the main window.

func becomeMain()

Informs the window that it has become the main window.

func resignMain()

Resigns the window’s main window status.

