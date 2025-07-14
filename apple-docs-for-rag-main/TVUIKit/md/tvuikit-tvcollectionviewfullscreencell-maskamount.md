

- TVUIKit
- TVCollectionViewFullScreenCell
-  maskAmount 

Instance Property

# maskAmount

The factor that determines the amount of masking applied on the cell.

tvOS 13.0+

``` source
@MainActor
var maskAmount: CGFloat { get }
```

## Discussion

The amount of masking is determined by attributes of the collection view. A value of 0.0 is applied automatically when the cell is in full screen mode, indicating that there is no masking around the cell. A value of 1.0 is the default masking applied in browsing mode.

## See Also

### Modifying Cell Appearance

var contentBleed: UIEdgeInsets

The amount of content that overlaps into the masked portions of the cell.

var cornerRadius: CGFloat

The radius to use when drawing rounded corners for the cell.

