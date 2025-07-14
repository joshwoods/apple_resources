

- AppKit
- NSWindow
-  contentRect(forFrameRect:styleMask:) 

Type Method

# contentRect(forFrameRect:styleMask:)

Returns the content rectangle used by a window with a given frame rectangle and window style.

macOS

``` source
@MainActor
class func contentRect(
    forFrameRect fRect: NSRect,
    styleMask style: NSWindow.StyleMask
) -> NSRect
```

## Parameters 

`fRect`  

The frame rectangle for the window expressed in screen coordinates.

`style`  

The window style for the window. See NSWindow.StyleMask for a list of style mask values.

## Return Value

The content rectangle, expressed in screen coordinates, used by the window with `fRect` and `style`.

## Discussion

When a `NSWindow` instance is available, you should use contentRect(forFrameRect:) instead of this method.

## See Also

### Getting Layout Information

class func frameRect(forContentRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the frame rectangle used by a window with a given content rectangle and window style.

class func minFrameWidth(withTitle: String, styleMask: NSWindow.StyleMask) -> CGFloat

Returns the minimum width a window’s frame rectangle must have for it to display a title, with a given window style.

func contentRect(forFrameRect: NSRect) -> NSRect

Returns the window’s content rectangle with a given frame rectangle.

func frameRect(forContentRect: NSRect) -> NSRect

Returns the window’s frame rectangle with a given content rectangle.

