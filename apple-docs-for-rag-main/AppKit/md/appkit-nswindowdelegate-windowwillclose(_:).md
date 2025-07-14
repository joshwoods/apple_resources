

- AppKit
- NSWindowDelegate
-  windowWillClose(\_:) 

Instance Method

# windowWillClose(\_:)

Tells the delegate that the window is about to close.

macOS 10.10+

``` source
@MainActor
optional func windowWillClose(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willCloseNotification.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

## See Also

### Closing Windows

func windowShouldClose(NSWindow) -> Bool

Tells the delegate that the user has attempted to close a window or the window has received a performClose(_:) message.

