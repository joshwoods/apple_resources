

- AppKit
- NSWindowDelegate
-  windowDidBecomeKey(\_:) 

Instance Method

# windowDidBecomeKey(\_:)

Tells the delegate that the window has become the key window.

macOS 10.10+

``` source
@MainActor
optional func windowDidBecomeKey(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didBecomeKeyNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

## See Also

### Managing Key Status

func windowDidResignKey(Notification)

Tells the delegate that the window has resigned key window status.

