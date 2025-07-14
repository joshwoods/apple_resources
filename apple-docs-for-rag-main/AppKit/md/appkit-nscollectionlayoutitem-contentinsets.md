

- AppKit
- NSCollectionLayoutItem
-  contentInsets 

Instance Property

# contentInsets

The amount of space added around the content of the item to adjust its final size after its position is computed.

macOS 10.15+

``` source
@MainActor
var contentInsets: NSDirectionalEdgeInsets { get set }
```

## Discussion

You can use this property within a grid layout to apply even spacing around each edge of each item. Content insets are applied after applying edgeSpacing.

The following diagram shows the result of applying 2 points of content insets to each edge of each item in a group.

Note

The value of this property is ignored for any axis that uses an estimated value for its dimension. For more information, see estimated(_:).

## See Also

### Configuring spacing and insets

var edgeSpacing: NSCollectionLayoutEdgeSpacing?

The amount of space added around the boundaries of the item between other items and this item’s container.

