

- AppKit
- NSWindow
-  contentRect(forFrameRect:) 

Instance Method

# contentRect(forFrameRect:)

Returns the window’s content rectangle with a given frame rectangle.

macOS

``` source
@MainActor
func contentRect(forFrameRect frameRect: NSRect) -> NSRect
```

## Parameters 

`frameRect`  

The frame rectangle for the window expressed in screen coordinates.

## Return Value

The window’s content rectangle, expressed in screen coordinates, with f`rameRect`.

## Discussion

The window uses its current style mask in computing the content rectangle. See NSWindow.StyleMask for a list of style mask values. The main advantage of this instance-method counterpart to contentRect(forFrameRect:styleMask:) is that it allows you to take toolbars into account when converting between content and frame rectangles. (The toolbar is not included in the content rectangle.)

## See Also

### Getting Layout Information

class func contentRect(forFrameRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the content rectangle used by a window with a given frame rectangle and window style.

class func frameRect(forContentRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the frame rectangle used by a window with a given content rectangle and window style.

class func minFrameWidth(withTitle: String, styleMask: NSWindow.StyleMask) -> CGFloat

Returns the minimum width a window’s frame rectangle must have for it to display a title, with a given window style.

func frameRect(forContentRect: NSRect) -> NSRect

Returns the window’s frame rectangle with a given content rectangle.

