

- AppKit
- NSScroller
-  knobStyle 

Instance Property

# knobStyle

The scroller’s knob style.

macOS 10.7+

``` source
@MainActor
var knobStyle: NSScroller.KnobStyle { get set }
```

## Discussion

The value of this property does not affect legacy scrollers. NSScroller.KnobStyle.default is appropriate for a wide range of content, but in some cases choosing an alternative knob style may enhance visibility of the scroller knob atop some kinds of content.

For a list of possible values, see NSScroller.KnobStyle.

## See Also

### Managing Presentation Style

class var preferredScrollerStyle: NSScroller.Style

Returns the style of scrollers that applications should use wherever possible.

var scrollerStyle: NSScroller.Style

The scroller style for this scroller.

