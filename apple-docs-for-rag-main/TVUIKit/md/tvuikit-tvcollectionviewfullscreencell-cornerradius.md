

- TVUIKit
- TVCollectionViewFullScreenCell
-  cornerRadius 

Instance Property

# cornerRadius

The radius to use when drawing rounded corners for the cell.

tvOS 13.0+

``` source
@MainActor
var cornerRadius: CGFloat { get }
```

## Discussion

Setting the radius to a value greater than 0.0 points applies increasingly rounded corners to the cell.

## See Also

### Modifying Cell Appearance

var contentBleed: UIEdgeInsets

The amount of content that overlaps into the masked portions of the cell.

var maskAmount: CGFloat

The factor that determines the amount of masking applied on the cell.

