

- TVUIKit
- TVCollectionViewFullScreenLayout
-  maskInset 

Instance Property

# maskInset

The edge insets of the cell mask.

tvOS 13.0+

``` source
@MainActor
var maskInset: UIEdgeInsets { get set }
```

## Discussion

Use the `maskInset` property to create a mask around the cell that is only revealed when the cell is brought into focus.

The default value of this property is `UIEdgeInsetsMake(32.0, 120.0, 0.0, 120.0)`.

## See Also

### Configuring cell masks

var maskAmount: CGFloat

The amount by which to mask the cells in a collection view.

