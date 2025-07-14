

- AppKit
- NSApplication
-  hide(\_:) 

Instance Method

# hide(\_:)

Hides all the receiver’s windows, and the next app in line is activated.

macOS

``` source
@MainActor
func hide(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

This method is usually invoked when the user chooses Hide in the app’s main menu. When this method begins, it posts an willHideNotification to the default notification center. When it completes successfully, it posts an didHideNotification.

## See Also

### Related Documentation

func miniaturizeAll(Any?)

Miniaturizes all the receiver’s windows.

func applicationDidHide(Notification)

Tells the delegate that the app is now hidden.

func applicationWillHide(Notification)

Tells the delegate that the app is about to be hidden.

### Hiding Windows

var isHidden: Bool

A Boolean value indicating whether the app is hidden.

func unhide(Any?)

Restores hidden windows to the screen and makes the receiver active.

func unhideWithoutActivation()

Restores hidden windows without activating their owner (the receiver).

