

- UIKit
- NSCollectionLayoutItem
-  edgeSpacing 

Instance Property

# edgeSpacing

The amount of space added around the boundaries of the item between other items and this item’s container.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var edgeSpacing: NSCollectionLayoutEdgeSpacing? { get set }
```

## Discussion

Use this property to adjust the position of the item in relation to its container and other items. For example, you can use this property to apply extra space to the trailing edge of each item. Edge spacing is applied before applying contentInsets.

The following diagram shows the result of applying 2 points of trailing edge spacing to the items in a group:

## See Also

### Configuring spacing and insets

var contentInsets: NSDirectionalEdgeInsets

The amount of space added around the content of the item to adjust its final size after its position is computed.

