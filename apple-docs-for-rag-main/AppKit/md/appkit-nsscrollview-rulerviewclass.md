

- AppKit
- NSScrollView
-  rulerViewClass 

Type Property

# rulerViewClass

Returns the default class to be used for ruler objects in NSScrollViews.

macOS

``` source
@MainActor
class var rulerViewClass: AnyClass! { get set }
```

## Discussion

This class is normally NSRulerView.

## See Also

### Managing Rulers

var hasHorizontalRuler: Bool

A Boolean that indicates whether the scroll view keeps a horizontal ruler object.

var horizontalRulerView: NSRulerView?

The scroll view’s horizontal ruler view.

var hasVerticalRuler: Bool

A Boolean that indicates whether the scroll view keeps a vertical ruler object.

var verticalRulerView: NSRulerView?

The scroll view’s vertical ruler view.

var rulersVisible: Bool

A Boolean that indicates whether the scroll view displays its rulers.

