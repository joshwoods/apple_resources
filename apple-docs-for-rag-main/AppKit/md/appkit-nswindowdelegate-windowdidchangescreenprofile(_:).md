

- AppKit
- NSWindowDelegate
-  windowDidChangeScreenProfile(\_:) 

Instance Method

# windowDidChangeScreenProfile(\_:)

Tells the delegate that the window has changed screen display profiles.

macOS 10.10+

``` source
@MainActor
optional func windowDidChangeScreenProfile(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didChangeScreenProfileNotification.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

If your app runs in macOS 10.7.3 or later, you should instead watch for the notification `NSWindowDidChangeBackingPropertiesNotification`.

## See Also

### Moving Windows

func windowWillMove(Notification)

Tells the delegate that the window is about to move.

func windowDidMove(Notification)

Tells the delegate that the window has moved.

func windowDidChangeScreen(Notification)

Tells the delegate that the window has changed screens.

func windowDidChangeBackingProperties(Notification)

Tells the delegate that the window backing properties changed.

