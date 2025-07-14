

- UIKit
- UIView
-  frame(forAlignmentRect:) 

Instance Method

# frame(forAlignmentRect:)

Returns the view’s frame for a given alignment rectangle.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func frame(forAlignmentRect alignmentRect: CGRect) -> CGRect
```

## Parameters 

`alignmentRect`  

The alignment rectangle whose corresponding frame is desired.

## Return Value

The frame for the specified alignment rectangle

## Discussion

The constraint-based layout system uses alignment rectangles to align views, rather than their frame. This allows custom views to be aligned based on the location of their content while still having a frame that encompasses any ornamentation they need to draw around their content, such as shadows or reflections.

The default implementation returns `alignmentRect` modified by the view’s alignmentRectInsets. Most custom views can override alignmentRectInsets to specify the location of their content within their frame. Custom views that require arbitrary transformations can override alignmentRect(forFrame:) and frame(forAlignmentRect:) to describe the location of their content. These two methods must always be inverses of each other.

## See Also

### Aligning views in Auto Layout

func alignmentRect(forFrame: CGRect) -> CGRect

Returns the view’s alignment rectangle for a given frame.

var alignmentRectInsets: UIEdgeInsets

The insets from the view’s frame that define its alignment rectangle.

var forFirstBaselineLayout: UIView

Returns a view used to satisfy first baseline constraints.

var forLastBaselineLayout: UIView

Returns a view used to satisfy last baseline constraints.

