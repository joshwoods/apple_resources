

- TVUIKit
- TVCollectionViewFullScreenCell
-  contentBleed 

Instance Property

# contentBleed

The amount of content that overlaps into the masked portions of the cell.

tvOS 13.0+

``` source
@MainActor
var contentBleed: UIEdgeInsets { get }
```

## Discussion

The portions of content that bleed into the masked portions go out of bounds, and consequently disappear from view.

## See Also

### Modifying Cell Appearance

var cornerRadius: CGFloat

The radius to use when drawing rounded corners for the cell.

var maskAmount: CGFloat

The factor that determines the amount of masking applied on the cell.

