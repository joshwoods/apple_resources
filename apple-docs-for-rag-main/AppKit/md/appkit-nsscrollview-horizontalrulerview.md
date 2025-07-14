

- AppKit
- NSScrollView
-  horizontalRulerView 

Instance Property

# horizontalRulerView

The scroll view’s horizontal ruler view.

macOS

``` source
@MainActor
var horizontalRulerView: NSRulerView? { get set }
```

## Discussion

The value of this property is `nil` when the scroll view has no horizontal ruler view.

If the scroll view is set to display a horizontal ruler view and doesn’t yet have one, this property creates an instance of the ruler view class set using the class method `setRulerViewClass(_:)`. You can use this property to override the default ruler class set using the class method `setRulerViewClass(_:)`.

Display of rulers is controlled using the rulersVisible property.

## See Also

### Managing Rulers

class var rulerViewClass: AnyClass!

Returns the default class to be used for ruler objects in NSScrollViews.

var hasHorizontalRuler: Bool

A Boolean that indicates whether the scroll view keeps a horizontal ruler object.

var hasVerticalRuler: Bool

A Boolean that indicates whether the scroll view keeps a vertical ruler object.

var verticalRulerView: NSRulerView?

The scroll view’s vertical ruler view.

var rulersVisible: Bool

A Boolean that indicates whether the scroll view displays its rulers.

