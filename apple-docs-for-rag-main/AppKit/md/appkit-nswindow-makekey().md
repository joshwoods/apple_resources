

- AppKit
- NSWindow
-  makeKey() 

Instance Method

# makeKey()

Makes the window the key window.

macOS

``` source
@MainActor
func makeKey()
```

## See Also

### Related Documentation

func makeMain()

Makes the window the main window.

### Managing Key Status

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window for the application.

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

func becomeKey()

Informs the window that it has become the key window.

func resignKey()

Resigns the window’s key window status.

