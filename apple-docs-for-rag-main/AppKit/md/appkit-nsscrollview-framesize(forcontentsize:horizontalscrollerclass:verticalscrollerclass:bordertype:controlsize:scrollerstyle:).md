

- AppKit
- NSScrollView
-  frameSize(forContentSize:horizontalScrollerClass:verticalScrollerClass:borderType:controlSize:scrollerStyle:) 

Type Method

# frameSize(forContentSize:horizontalScrollerClass:verticalScrollerClass:borderType:controlSize:scrollerStyle:)

Returns the frame size of a scroll view that contains a content view with the specified size.

macOS 10.7+

``` source
@MainActor
class func frameSize(
    forContentSize cSize: NSSize,
    horizontalScrollerClass: AnyClass?,
    verticalScrollerClass: AnyClass?,
    borderType type: NSBorderType,
    controlSize: NSControl.ControlSize,
    scrollerStyle: NSScroller.Style
) -> NSSize
```

## Parameters 

`cSize`  

The content size.

`horizontalScrollerClass`  

The class used as the horizontal scroller. A value of `nil` specifies that no horizontal scroller is used.

`verticalScrollerClass`  

The class used as the vertical scroller. A value of `nil` specifies that no horizontal scroller is used.

`type`  

Specifies the appearance of the style of the scroll view’s border. See NSBorderType for a list of possible values.

`controlSize`  

The control size. The possible values are specified in NSControl.ControlSize. NSMiniControlSize is not supported.

`scrollerStyle`  

Specifies the scroll style. See NSScroller.Style for supported values.

## Return Value

The size of the frame for the specified `contentSize`.

## Discussion

For an existing scroll view, you can simply use the `frame` method and extract its size.

## See Also

### Related Documentation

Scroll View Programming Guide for Mac

### Calculating Layout

class func contentSize(forFrameSize: NSSize, horizontalScrollerClass: AnyClass?, verticalScrollerClass: AnyClass?, borderType: NSBorderType, controlSize: NSControl.ControlSize, scrollerStyle: NSScroller.Style) -> NSSize

Returns the content size calculated from the frame size and the specified specifications.

