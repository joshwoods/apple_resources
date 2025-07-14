

- AppKit
- NSWindow
-  frameRect(forContentRect:) 

Instance Method

# frameRect(forContentRect:)

Returns the window’s frame rectangle with a given content rectangle.

macOS

``` source
@MainActor
func frameRect(forContentRect contentRect: NSRect) -> NSRect
```

## Parameters 

`contentRect`  

The content rectangle for the window expressed in screen coordinates.

## Return Value

The window’s frame rectangle, expressed in screen coordinates, with `contentRect`.

## Discussion

The window uses its current style mask in computing the frame rectangle. See NSWindow.StyleMask for a list of style mask values. The major advantage of this instance-method counterpart to frameRect(forContentRect:styleMask:) is that it allows you to take toolbars into account when converting between content and frame rectangles. (The toolbar is included in the frame rectangle but not the content rectangle.)

## See Also

### Getting Layout Information

class func contentRect(forFrameRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the content rectangle used by a window with a given frame rectangle and window style.

class func frameRect(forContentRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the frame rectangle used by a window with a given content rectangle and window style.

class func minFrameWidth(withTitle: String, styleMask: NSWindow.StyleMask) -> CGFloat

Returns the minimum width a window’s frame rectangle must have for it to display a title, with a given window style.

func contentRect(forFrameRect: NSRect) -> NSRect

Returns the window’s content rectangle with a given frame rectangle.

