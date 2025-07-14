

- AppKit
- NSWindowDelegate
-  windowDidExpose(\_:) 

Instance Method

# windowDidExpose(\_:)

Tells the delegate that the window has been exposed.

macOS 10.10+

``` source
@MainActor
optional func windowDidExpose(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didExposeNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

