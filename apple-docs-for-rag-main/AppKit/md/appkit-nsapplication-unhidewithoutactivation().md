

- AppKit
- NSApplication
-  unhideWithoutActivation() 

Instance Method

# unhideWithoutActivation()

Restores hidden windows without activating their owner (the receiver).

macOS

``` source
@MainActor
func unhideWithoutActivation()
```

## Discussion

When this method begins, it posts an willUnhideNotification to the default notification center. If it completes successfully, it posts an didUnhideNotification.

## See Also

### Related Documentation

func activate(ignoringOtherApps: Bool)

Makes the receiver the active app.

Deprecated

func applicationDidUnhide(Notification)

Tells the delegate that the app is now visible.

func applicationWillUnhide(Notification)

Tells the delegate that the app is about to become visible.

### Hiding Windows

var isHidden: Bool

A Boolean value indicating whether the app is hidden.

func hide(Any?)

Hides all the receiver’s windows, and the next app in line is activated.

func unhide(Any?)

Restores hidden windows to the screen and makes the receiver active.

