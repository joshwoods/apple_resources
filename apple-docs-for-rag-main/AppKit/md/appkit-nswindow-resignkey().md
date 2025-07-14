

- AppKit
- NSWindow
-  resignKey() 

Instance Method

# resignKey()

Resigns the window’s key window status.

macOS

``` source
@MainActor
func resignKey()
```

## Discussion

This method sends resignKey() to the window’s first responder, sends windowDidResignKey(_:) to the window’s delegate, and posts didResignKeyNotification to the default notification center.

Never invoke this method directly.

## See Also

### Related Documentation

func resignMain()

Resigns the window’s main window status.

### Managing Key Status

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window for the application.

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKey()

Makes the window the key window.

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

func becomeKey()

Informs the window that it has become the key window.

