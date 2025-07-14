

- AppKit
- NSWindowDelegate
-  windowDidChangeScreen(\_:) 

Instance Method

# windowDidChangeScreen(\_:)

Tells the delegate that the window has changed screens.

macOS 10.10+

``` source
@MainActor
optional func windowDidChangeScreen(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didChangeScreenNotification.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

## See Also

### Moving Windows

func windowWillMove(Notification)

Tells the delegate that the window is about to move.

func windowDidMove(Notification)

Tells the delegate that the window has moved.

func windowDidChangeScreenProfile(Notification)

Tells the delegate that the window has changed screen display profiles.

func windowDidChangeBackingProperties(Notification)

Tells the delegate that the window backing properties changed.

