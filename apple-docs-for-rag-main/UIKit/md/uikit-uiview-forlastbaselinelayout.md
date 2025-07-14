

- UIKit
- UIView
-  forLastBaselineLayout 

Instance Property

# forLastBaselineLayout

Returns a view used to satisfy last baseline constraints.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var forLastBaselineLayout: UIView { get }
```

## Discussion

For views with multiple rows of text, the last baseline is the baseline for the bottommost row.

When you make a constraint to a view’s NSLayoutConstraint.Attribute.lastBaseline attribute, Auto Layout uses the baseline of the view returned by this method. If that view does not have a baseline, Auto Layout uses the view’s bottom edge.

Override this property to return a text-based subview (for example, UILabel or a nonscrolling UITextView). The returned view must be a subview of the receiver. The default implementation returns the receiving view.

## See Also

### Aligning views in Auto Layout

func alignmentRect(forFrame: CGRect) -> CGRect

Returns the view’s alignment rectangle for a given frame.

func frame(forAlignmentRect: CGRect) -> CGRect

Returns the view’s frame for a given alignment rectangle.

var alignmentRectInsets: UIEdgeInsets

The insets from the view’s frame that define its alignment rectangle.

var forFirstBaselineLayout: UIView

Returns a view used to satisfy first baseline constraints.

