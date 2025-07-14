

- AppKit
- NSWindowDelegate
-  windowDidUpdate(\_:) 

Instance Method

# windowDidUpdate(\_:)

Tells the delegate that the window received an update() message.

macOS 10.10+

``` source
@MainActor
optional func windowDidUpdate(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didUpdateNotification

## Discussion

You can retrieve the window object in question by sending object to `notification`.

