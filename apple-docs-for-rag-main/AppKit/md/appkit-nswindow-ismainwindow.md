

- AppKit
- NSWindow
-  isMainWindow 

Instance Property

# isMainWindow

A Boolean value that indicates whether the window is the application’s main window.

macOS

``` source
@MainActor
var isMainWindow: Bool { get }
```

## Discussion

The value of this property is true when the window is the main window for the application; otherwise, false.

## See Also

### Related Documentation

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window for the application.

### Managing Main Status

var canBecomeMain: Bool

A Boolean value that indicates whether the window can become the application’s main window.

func makeMain()

Makes the window the main window.

func becomeMain()

Informs the window that it has become the main window.

func resignMain()

Resigns the window’s main window status.

