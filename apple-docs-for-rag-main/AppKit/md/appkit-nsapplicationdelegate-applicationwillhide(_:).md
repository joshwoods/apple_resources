

- AppKit
- NSApplicationDelegate
-  applicationWillHide(\_:) 

Instance Method

# applicationWillHide(\_:)

Tells the delegate that the app is about to be hidden.

macOS 10.10+

``` source
@MainActor
optional func applicationWillHide(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willHideNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Related Documentation

func hide(Any?)

Hides all the receiver’s windows, and the next app in line is activated.

### Hiding Applications

func applicationDidHide(Notification)

Tells the delegate that the app is now hidden.

func applicationWillUnhide(Notification)

Tells the delegate that the app is about to become visible.

func applicationDidUnhide(Notification)

Tells the delegate that the app is now visible.

