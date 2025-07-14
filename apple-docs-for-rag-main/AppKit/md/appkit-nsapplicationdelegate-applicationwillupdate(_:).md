

- AppKit
- NSApplicationDelegate
-  applicationWillUpdate(\_:) 

Instance Method

# applicationWillUpdate(\_:)

Tells the delegate that the app is about to update its windows.

macOS 10.10+

``` source
@MainActor
optional func applicationWillUpdate(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willUpdateNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Related Documentation

func updateWindows()

Sends an update() message to each onscreen window.

### Managing Windows

func applicationDidUpdate(Notification)

Tells the delegate that the app’s windows did update.

func applicationShouldHandleReopen(NSApplication, hasVisibleWindows: Bool) -> Bool

Returns a Boolean value that indicates if the app responds to reopen AppleEvents.

