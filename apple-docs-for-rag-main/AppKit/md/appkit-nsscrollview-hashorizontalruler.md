

- AppKit
- NSScrollView
-  hasHorizontalRuler 

Instance Property

# hasHorizontalRuler

A Boolean that indicates whether the scroll view keeps a horizontal ruler object.

macOS

``` source
@MainActor
var hasHorizontalRuler: Bool { get set }
```

## Discussion

When the value of this method is true, the scroll view allocates a horizontal ruler the first time it’s needed.

Display of rulers is controlled using the rulersVisible property.

## See Also

### Managing Rulers

class var rulerViewClass: AnyClass!

Returns the default class to be used for ruler objects in NSScrollViews.

var horizontalRulerView: NSRulerView?

The scroll view’s horizontal ruler view.

var hasVerticalRuler: Bool

A Boolean that indicates whether the scroll view keeps a vertical ruler object.

var verticalRulerView: NSRulerView?

The scroll view’s vertical ruler view.

var rulersVisible: Bool

A Boolean that indicates whether the scroll view displays its rulers.

