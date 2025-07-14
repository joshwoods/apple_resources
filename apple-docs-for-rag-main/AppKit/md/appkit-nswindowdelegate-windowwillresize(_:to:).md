

- AppKit
- NSWindowDelegate
-  windowWillResize(\_:to:) 

Instance Method

# windowWillResize(\_:to:)

Tells the delegate that the window is being resized (whether by the user or through one of the `setFrame...` methods other than setFrame(_:display:)).

macOS

``` source
@MainActor
optional func windowWillResize(
    _ sender: NSWindow,
    to frameSize: NSSize
) -> NSSize
```

## Parameters 

`sender`  

The window being resized.

`frameSize`  

The size to which the specified window is being resized.

## Return Value

A custom size to which the specified window will be resized.

## Discussion

The `frameSize` contains the size (in screen coordinates) `sender` will be resized to. To resize to a different size, simply return the desired size from this method; to avoid resizing, return the current size. `sender`’s minimum and maximum size constraints have already been applied when this method is called.

While the user is resizing a window, the delegate is sent a series of windowWillResize(_:to:) messages as the window’s frame continues to change size.

## See Also

### Sizing Windows

func windowDidResize(Notification)

Tells the delegate that the window has been resized.

func windowWillStartLiveResize(Notification)

Tells the delegate that the window is about to be live resized.

func windowDidEndLiveResize(Notification)

Tells the delegate that a live resize operation on the window has ended.

