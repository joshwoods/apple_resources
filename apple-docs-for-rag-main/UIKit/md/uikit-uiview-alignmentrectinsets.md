

- UIKit
- UIView
-  alignmentRectInsets 

Instance Property

# alignmentRectInsets

The insets from the view’s frame that define its alignment rectangle.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var alignmentRectInsets: UIEdgeInsets { get }
```

## Discussion

The default value of this property is an UIEdgeInsets structure with zero values. Custom views that draw ornamentation around their content should use this property to return insets that align with the edges of the content, excluding the ornamentation. This allows the constraint-based layout system to align views based on their content, rather than just their frame.

Custom views whose content location can’t be expressed by a simple set of insets should override alignmentRect(forFrame:) and frame(forAlignmentRect:) to describe their custom transform between alignment rectangle and frame.

## See Also

### Aligning views in Auto Layout

func alignmentRect(forFrame: CGRect) -> CGRect

Returns the view’s alignment rectangle for a given frame.

func frame(forAlignmentRect: CGRect) -> CGRect

Returns the view’s frame for a given alignment rectangle.

var forFirstBaselineLayout: UIView

Returns a view used to satisfy first baseline constraints.

var forLastBaselineLayout: UIView

Returns a view used to satisfy last baseline constraints.

