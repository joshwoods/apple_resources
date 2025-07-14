

- AppKit
- NSWindowDelegate
-  windowDidResignMain(\_:) 

Instance Method

# windowDidResignMain(\_:)

Tells the delegate that the window has resigned main window status.

macOS 10.10+

``` source
@MainActor
optional func windowDidResignMain(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didResignMainNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

## See Also

### Managing Main Status

func windowDidBecomeMain(Notification)

Tells the delegate that the window has become main.

