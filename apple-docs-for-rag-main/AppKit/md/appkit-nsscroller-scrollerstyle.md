

- AppKit
- NSScroller
-  scrollerStyle 

Instance Property

# scrollerStyle

The scroller style for this scroller.

macOS 10.7+

``` source
@MainActor
var scrollerStyle: NSScroller.Style { get set }
```

## Discussion

For a scroller that’s managed by an NSScrollView object, the setter is automatically invoked by the scroll view with the appropriate setting, according to the user’s Appearance preference settings and possibly what pointing device(s) are present (see preferredScrollerStyle).

For a list of valid scroller styles, see NSScroller.Style.

## See Also

### Managing Presentation Style

class var preferredScrollerStyle: NSScroller.Style

Returns the style of scrollers that applications should use wherever possible.

var knobStyle: NSScroller.KnobStyle

The scroller’s knob style.

