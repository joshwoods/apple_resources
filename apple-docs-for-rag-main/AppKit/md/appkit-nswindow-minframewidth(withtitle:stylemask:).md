

- AppKit
- NSWindow
-  minFrameWidth(withTitle:styleMask:) 

Type Method

# minFrameWidth(withTitle:styleMask:)

Returns the minimum width a window’s frame rectangle must have for it to display a title, with a given window style.

macOS

``` source
@MainActor
class func minFrameWidth(
    withTitle title: String,
    styleMask style: NSWindow.StyleMask
) -> CGFloat
```

## Parameters 

`title`  

The title for the window.

`style`  

The window style for the window. See NSWindow.StyleMask for a list of style mask values.

## Return Value

The minimum width of the window’s frame, using `style`, in order to display `title`.

## See Also

### Getting Layout Information

class func contentRect(forFrameRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the content rectangle used by a window with a given frame rectangle and window style.

class func frameRect(forContentRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the frame rectangle used by a window with a given content rectangle and window style.

func contentRect(forFrameRect: NSRect) -> NSRect

Returns the window’s content rectangle with a given frame rectangle.

func frameRect(forContentRect: NSRect) -> NSRect

Returns the window’s frame rectangle with a given content rectangle.

