

- AppKit
- NSWindow
-  update() 

Instance Method

# update()

Updates the window.

macOS

``` source
@MainActor
func update()
```

## Discussion

The `NSWindow` implementation of this method does nothing more than post an didUpdateNotification notification to the default notification center. A subclass can override this method to perform specialized operations, but it should send an update message to `super` just before returning. For example, the `NSMenu` class implements this method to disable and enable menu commands.

An `NSWindow` object is automatically sent an `update` message on every pass through the event loop and before it’s displayed onscreen. You can manually cause an `update` message to be sent to all visible `NSWindow` objects through the `NSApplication` updateWindows() method.

## See Also

### Related Documentation

func setWindowsNeedUpdate(Bool)

Sets whether the receiver’s windows need updating when the receiver has finished processing the current event.

### Updating Windows

func disableScreenUpdatesUntilFlush()

Disables the window’s screen updates until the window is flushed.

Deprecated

