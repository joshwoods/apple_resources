

- AppKit
- NSWindowDelegate
-  windowDidBecomeMain(\_:) 

Instance Method

# windowDidBecomeMain(\_:)

Tells the delegate that the window has become main.

macOS 10.10+

``` source
@MainActor
optional func windowDidBecomeMain(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didBecomeMainNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

## See Also

### Managing Main Status

func windowDidResignMain(Notification)

Tells the delegate that the window has resigned main window status.

