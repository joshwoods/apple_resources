

- AppKit
- NSWindowDelegate
-  windowDidMove(\_:) 

Instance Method

# windowDidMove(\_:)

Tells the delegate that the window has moved.

macOS 10.10+

``` source
@MainActor
optional func windowDidMove(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didMoveNotification.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

## See Also

### Moving Windows

func windowWillMove(Notification)

Tells the delegate that the window is about to move.

func windowDidChangeScreen(Notification)

Tells the delegate that the window has changed screens.

func windowDidChangeScreenProfile(Notification)

Tells the delegate that the window has changed screen display profiles.

func windowDidChangeBackingProperties(Notification)

Tells the delegate that the window backing properties changed.

