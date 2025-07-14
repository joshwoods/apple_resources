

- AppKit
- NSWindow
-  becomeMain() 

Instance Method

# becomeMain()

Informs the window that it has become the main window.

macOS

``` source
@MainActor
func becomeMain()
```

## Discussion

This method posts an didBecomeMainNotification to the default notification center.

Never invoke this method directly.

## See Also

### Related Documentation

func becomeKey()

Informs the window that it has become the key window.

### Managing Main Status

var isMainWindow: Bool

A Boolean value that indicates whether the window is the application’s main window.

var canBecomeMain: Bool

A Boolean value that indicates whether the window can become the application’s main window.

func makeMain()

Makes the window the main window.

func resignMain()

Resigns the window’s main window status.

