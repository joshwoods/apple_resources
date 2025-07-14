

- AppKit
- NSScroller
-  controlSize 

Instance Property

# controlSize

The size of the scroller.

macOS

``` source
@MainActor
var controlSize: NSControl.ControlSize { get set }
```

## Discussion

Valid values for `controlSize` are described in NSControl.ControlSize (`NSCell`).

## See Also

### Determining Scroller Size

class func scrollerWidth(for: NSControl.ControlSize, scrollerStyle: NSScroller.Style) -> CGFloat

Returns the width for scrollers of the receiving class for a given control size and scroller style.

