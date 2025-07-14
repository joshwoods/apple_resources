

- AppKit
- NSWindow
-  canBecomeKey 

Instance Property

# canBecomeKey

A Boolean value that indicates whether the window can become the key window.

macOS

``` source
@MainActor
var canBecomeKey: Bool { get }
```

## Discussion

The value of this property is true if the window can become the key window, otherwise, false.

Attempts to make the window the key window are abandoned if the value of this property is false. The value of this property is true if the window has a title bar or a resize bar, or false otherwise.

## See Also

### Managing Key Status

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window for the application.

func makeKey()

Makes the window the key window.

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

func becomeKey()

Informs the window that it has become the key window.

func resignKey()

Resigns the window’s key window status.

