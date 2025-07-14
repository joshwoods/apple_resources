

- AppKit
- NSWindow
-  isKeyWindow 

Instance Property

# isKeyWindow

A Boolean value that indicates whether the window is the key window for the application.

macOS

``` source
@MainActor
var isKeyWindow: Bool { get }
```

## Discussion

The value of this property is true if the window is the key window for the application; otherwise, false.

## See Also

### Related Documentation

var isMainWindow: Bool

A Boolean value that indicates whether the window is the application’s main window.

### Managing Key Status

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKey()

Makes the window the key window.

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

func becomeKey()

Informs the window that it has become the key window.

func resignKey()

Resigns the window’s key window status.

