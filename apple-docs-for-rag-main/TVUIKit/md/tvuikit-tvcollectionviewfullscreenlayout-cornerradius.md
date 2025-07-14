

- TVUIKit
- TVCollectionViewFullScreenLayout
-  cornerRadius 

Instance Property

# cornerRadius

The radius to use when drawing rounded corners for the cell.

tvOS 13.0+

``` source
@MainActor
var cornerRadius: CGFloat { get set }
```

## Discussion

Setting the radius to a value greater than 0.0 points applies increasingly rounded corners on the cell.

The default value of this property is 36.0 points.

