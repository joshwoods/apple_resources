

- AppKit
- NSWindow
-  makeMain() 

Instance Method

# makeMain()

Makes the window the main window.

macOS

``` source
@MainActor
func makeMain()
```

## See Also

### Related Documentation

func makeKey()

Makes the window the key window.

### Managing Main Status

var isMainWindow: Bool

A Boolean value that indicates whether the window is the application’s main window.

var canBecomeMain: Bool

A Boolean value that indicates whether the window can become the application’s main window.

func becomeMain()

Informs the window that it has become the main window.

func resignMain()

Resigns the window’s main window status.

