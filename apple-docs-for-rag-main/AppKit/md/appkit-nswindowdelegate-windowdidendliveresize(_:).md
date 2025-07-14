

- AppKit
- NSWindowDelegate
-  windowDidEndLiveResize(\_:) 

Instance Method

# windowDidEndLiveResize(\_:)

Tells the delegate that a live resize operation on the window has ended.

macOS 10.6+

``` source
@MainActor
optional func windowDidEndLiveResize(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didEndLiveResizeNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

## See Also

### Sizing Windows

func windowWillResize(NSWindow, to: NSSize) -> NSSize

Tells the delegate that the window is being resized (whether by the user or through one of the `setFrame...` methods other than setFrame(_:display:)).

func windowDidResize(Notification)

Tells the delegate that the window has been resized.

func windowWillStartLiveResize(Notification)

Tells the delegate that the window is about to be live resized.

