

- AppKit
- NSWindow
-  disableScreenUpdatesUntilFlush() Deprecated

Instance Method

# disableScreenUpdatesUntilFlush()

Disables the window’s screen updates until the window is flushed.

macOS 10.0–15.0Deprecated

``` source
@MainActor
func disableScreenUpdatesUntilFlush()
```

Deprecated

This method does not do anything and should not be called.

## Discussion

This method can be invoked to synchronize hardware surface flushes with the window’s flushes. The window immediately disables screen updates using the NSDisableScreenUpdates() function and reenables screen updates when the window flushes. Sending this message multiple times during a window update cycle has no effect.

To ensure that screen updates are reenabled in a timely manner, it’s crucial that the window is marked as needing display and that the display will occur soon (that is, within the next second). When you invoke `disableScreenUpdatesUntilFlush`, you can make sure that a marked window gets displayed by returning control to the run loop on the main thread or by sending the window displayIfNeeded() or display(). If it’s unclear whether the window is marked as needing display, you can also ensure that a display occurs by using setNeedsDisplay(_:) for a view that’s visible in the window.

## See Also

### Updating Windows

func update()

Updates the window.

