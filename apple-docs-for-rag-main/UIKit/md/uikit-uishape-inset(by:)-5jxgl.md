

- UIKit
- UIShape
-  inset(by:) 

Instance Method

# inset(by:)

Creates a new modified shape by applying the provided insets to this shape.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
func inset(by insets: UIEdgeInsets) -> UIShape
```

## Discussion

You can use negative values to add inner padding to a shape.

If it isn’t possible to inset this shape (for example, if it’s a custom path), this method doesn’t have any effect. For some shapes like rounded rectangles, this method can also modify the corner radii of the shape to ensure the resulting corners are concentric.

## See Also

### Creating a shape by applying insets

func inset(by: CGFloat) -> UIShape

Creates a new modified shape by applying the provided inset to this shape.

