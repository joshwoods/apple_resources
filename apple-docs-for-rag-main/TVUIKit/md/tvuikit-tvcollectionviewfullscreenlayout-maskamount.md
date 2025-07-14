

- TVUIKit
- TVCollectionViewFullScreenLayout
-  maskAmount 

Instance Property

# maskAmount

The amount by which to mask the cells in a collection view.

tvOS 13.0+

``` source
@MainActor
var maskAmount: CGFloat { get set }
```

## Discussion

Use the `maskAmount` property to change how much masking the collection view applies to its cells. Setting the value of the property on the layout updates the `maskAmount` value of all the cells.

This property can take on a float value between `0` and `1.0`. A value of `0` indicates that the cells are full-screen, and a value of `1.0` indicates that the collection view applies the full mask to its cells.

The default value of this property is `1.0`.

## See Also

### Configuring cell masks

var maskInset: UIEdgeInsets

The edge insets of the cell mask.

