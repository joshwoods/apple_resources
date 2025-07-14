

- AppKit
- NSScroller
-  scrollerWidth(for:scrollerStyle:) 

Type Method

# scrollerWidth(for:scrollerStyle:)

Returns the width for scrollers of the receiving class for a given control size and scroller style.

macOS 10.7+

``` source
@MainActor
class func scrollerWidth(
    for controlSize: NSControl.ControlSize,
    scrollerStyle: NSScroller.Style
) -> CGFloat
```

## Parameters 

`controlSize`  

A control size.

`scrollerStyle`  

A scroller style.

## Return Value

The width for scrollers of the receiving class for `controlSize` and `scrollerStyle`.

## Discussion

You should use this method in preference to scrollerWidthForControlSize:, which assumes a scroller style of NSScroller.Style.legacy, and scrollerWidth which in addition assumes a control size of NSRegularControlSize.

## See Also

### Determining Scroller Size

var controlSize: NSControl.ControlSize

The size of the scroller.

