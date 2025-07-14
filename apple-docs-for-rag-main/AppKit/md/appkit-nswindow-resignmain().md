

- AppKit
- NSWindow
-  resignMain() 

Instance Method

# resignMain()

Resigns the window’s main window status.

macOS

``` source
@MainActor
func resignMain()
```

## Discussion

This method sends windowDidResignMain(_:) to the window’s delegate and posts didResignMainNotification to the default notification center.

Never invoke this method directly.

## See Also

### Related Documentation

func resignKey()

Resigns the window’s key window status.

### Managing Main Status

var isMainWindow: Bool

A Boolean value that indicates whether the window is the application’s main window.

var canBecomeMain: Bool

A Boolean value that indicates whether the window can become the application’s main window.

func makeMain()

Makes the window the main window.

func becomeMain()

Informs the window that it has become the main window.

