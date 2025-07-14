

- AppKit
- NSDrawerDelegate
-  drawerWillResizeContents(\_:to:) Deprecated

Instance Method

# drawerWillResizeContents(\_:to:)

Invoked when the user resizes the drawer or parent.

macOS 10.0–10.13Deprecated

``` source
optional func drawerWillResizeContents(
    _ sender: NSDrawer,
    to contentSize: NSSize
) -> NSSize
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`sender`  

The drawer being resized.

`contentSize`  

The proposed new size of the drawer.

## Return Value

The size that the drawer should be resized to. To resize to a different size, simply return the desired size from this method; to avoid resizing, return the current size.

## Discussion

The receiver’s minimum and maximum size constraints have already been applied when this method is invoked. While the user is resizing an `NSDrawer` or its parent, the delegate is sent a series of `windowWillResize` messages as the `NSDrawer` or parent window is dragged.

