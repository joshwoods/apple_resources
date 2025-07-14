

- AppKit
- NSApplicationDelegate
-  applicationDidUnhide(\_:) 

Instance Method

# applicationDidUnhide(\_:)

Tells the delegate that the app is now visible.

macOS 10.10+

``` source
@MainActor
optional func applicationDidUnhide(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didUnhideNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Related Documentation

func unhide(Any?)

Restores hidden windows to the screen and makes the receiver active.

### Hiding Applications

func applicationWillHide(Notification)

Tells the delegate that the app is about to be hidden.

func applicationDidHide(Notification)

Tells the delegate that the app is now hidden.

func applicationWillUnhide(Notification)

Tells the delegate that the app is about to become visible.

