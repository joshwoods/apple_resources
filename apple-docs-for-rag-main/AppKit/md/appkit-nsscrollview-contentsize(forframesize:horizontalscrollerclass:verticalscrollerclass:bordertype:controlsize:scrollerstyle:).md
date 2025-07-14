

- AppKit
- NSScrollView
-  contentSize(forFrameSize:horizontalScrollerClass:verticalScrollerClass:borderType:controlSize:scrollerStyle:) 

Type Method

# contentSize(forFrameSize:horizontalScrollerClass:verticalScrollerClass:borderType:controlSize:scrollerStyle:)

Returns the content size calculated from the frame size and the specified specifications.

macOS 10.7+

``` source
@MainActor
class func contentSize(
    forFrameSize fSize: NSSize,
    horizontalScrollerClass: AnyClass?,
    verticalScrollerClass: AnyClass?,
    borderType type: NSBorderType,
    controlSize: NSControl.ControlSize,
    scrollerStyle: NSScroller.Style
) -> NSSize
```

## Parameters 

`fSize`  

The frame size in screen coordinates.

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

The content view frame size.

## Discussion

For an existing scroll view, you can simply use the contentSize property.

## See Also

### Calculating Layout

class func frameSize(forContentSize: NSSize, horizontalScrollerClass: AnyClass?, verticalScrollerClass: AnyClass?, borderType: NSBorderType, controlSize: NSControl.ControlSize, scrollerStyle: NSScroller.Style) -> NSSize

Returns the frame size of a scroll view that contains a content view with the specified size.

