

- AppKit
- NSApplicationDelegate
-  applicationWillUnhide(\_:) 

Instance Method

# applicationWillUnhide(\_:)

Tells the delegate that the app is about to become visible.

macOS 10.10+

``` source
@MainActor
optional func applicationWillUnhide(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willUnhideNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Related Documentation

func unhide(Any?)

Restores hidden windows to the screen and makes the receiver active.

### Hiding Applications

func applicationWillHide(Notification)

Tells the delegate that the app is about to be hidden.

func applicationDidHide(Notification)

Tells the delegate that the app is now hidden.

func applicationDidUnhide(Notification)

Tells the delegate that the app is now visible.

