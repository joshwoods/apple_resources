

- AppKit
- NSScrollView
-  rulersVisible 

Instance Property

# rulersVisible

A Boolean that indicates whether the scroll view displays its rulers.

macOS

``` source
@MainActor
var rulersVisible: Bool { get set }
```

## Discussion

When the value of this property is true, the scroll view displays its rulers (creating them if needed). When the value of this property is false, the scroll view doesn’t display its rulers.

## See Also

### Managing Rulers

class var rulerViewClass: AnyClass!

Returns the default class to be used for ruler objects in NSScrollViews.

var hasHorizontalRuler: Bool

A Boolean that indicates whether the scroll view keeps a horizontal ruler object.

var horizontalRulerView: NSRulerView?

The scroll view’s horizontal ruler view.

var hasVerticalRuler: Bool

A Boolean that indicates whether the scroll view keeps a vertical ruler object.

var verticalRulerView: NSRulerView?

The scroll view’s vertical ruler view.

