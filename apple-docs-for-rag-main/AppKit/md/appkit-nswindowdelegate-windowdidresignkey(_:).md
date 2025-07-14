

- AppKit
- NSWindowDelegate
-  windowDidResignKey(\_:) 

Instance Method

# windowDidResignKey(\_:)

Tells the delegate that the window has resigned key window status.

macOS 10.10+

``` source
@MainActor
optional func windowDidResignKey(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didResignKeyNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

## See Also

### Managing Key Status

func windowDidBecomeKey(Notification)

Tells the delegate that the window has become the key window.

