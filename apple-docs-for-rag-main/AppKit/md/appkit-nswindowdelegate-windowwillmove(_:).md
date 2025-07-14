

- AppKit
- NSWindowDelegate
-  windowWillMove(\_:) 

Instance Method

# windowWillMove(\_:)

Tells the delegate that the window is about to move.

macOS 10.10+

``` source
@MainActor
optional func windowWillMove(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willMoveNotification.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

## See Also

### Moving Windows

func windowDidMove(Notification)

Tells the delegate that the window has moved.

func windowDidChangeScreen(Notification)

Tells the delegate that the window has changed screens.

func windowDidChangeScreenProfile(Notification)

Tells the delegate that the window has changed screen display profiles.

func windowDidChangeBackingProperties(Notification)

Tells the delegate that the window backing properties changed.

