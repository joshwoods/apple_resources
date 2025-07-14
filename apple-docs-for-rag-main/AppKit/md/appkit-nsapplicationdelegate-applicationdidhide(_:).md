

- AppKit
- NSApplicationDelegate
-  applicationDidHide(\_:) 

Instance Method

# applicationDidHide(\_:)

Tells the delegate that the app is now hidden.

macOS 10.10+

``` source
@MainActor
optional func applicationDidHide(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didHideNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Related Documentation

func unhide(Any?)

Restores hidden windows to the screen and makes the receiver active.

### Hiding Applications

func applicationWillHide(Notification)

Tells the delegate that the app is about to be hidden.

func applicationWillUnhide(Notification)

Tells the delegate that the app is about to become visible.

func applicationDidUnhide(Notification)

Tells the delegate that the app is now visible.

