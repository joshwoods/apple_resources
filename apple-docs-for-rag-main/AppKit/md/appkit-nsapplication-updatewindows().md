

- AppKit
- NSApplication
-  updateWindows() 

Instance Method

# updateWindows()

Sends an update() message to each onscreen window.

macOS

``` source
@MainActor
func updateWindows()
```

## Discussion

This method is invoked automatically in the main event loop after each event when running in `NSDefaultRunLoopMode` or `NSModalRunLoopMode`. This method is not invoked automatically when running in `NSEventTrackingRunLoopMode`.

When this method begins, it posts an willUpdateNotification to the default notification center. When it successfully completes, it posts an didUpdateNotification.

## See Also

### Related Documentation

func applicationDidUpdate(Notification)

Tells the delegate that the app’s windows did update.

func applicationWillUpdate(Notification)

Tells the delegate that the app is about to update its windows.

func update()

Updates the window.

### Updating Windows

func setWindowsNeedUpdate(Bool)

Sets whether the receiver’s windows need updating when the receiver has finished processing the current event.

