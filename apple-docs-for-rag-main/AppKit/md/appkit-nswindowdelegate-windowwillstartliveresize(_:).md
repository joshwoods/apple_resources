

- AppKit
- NSWindowDelegate
-  windowWillStartLiveResize(\_:) 

Instance Method

# windowWillStartLiveResize(\_:)

Tells the delegate that the window is about to be live resized.

macOS 10.6+

``` source
@MainActor
optional func windowWillStartLiveResize(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willStartLiveResizeNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

## See Also

### Sizing Windows

func windowWillResize(NSWindow, to: NSSize) -> NSSize

Tells the delegate that the window is being resized (whether by the user or through one of the `setFrame...` methods other than setFrame(_:display:)).

func windowDidResize(Notification)

Tells the delegate that the window has been resized.

func windowDidEndLiveResize(Notification)

Tells the delegate that a live resize operation on the window has ended.

