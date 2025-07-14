

- UIKit
- UICollectionLayoutListConfiguration
-  itemSeparatorHandler 

Instance Property

# itemSeparatorHandler

The closure that provides granular control over the list separator appearance of each item.

iOS 14.5+iPadOS 14.5+Mac CatalystvisionOS

``` source
var itemSeparatorHandler: UICollectionLayoutListConfiguration.ItemSeparatorHandler? { get set }
```

## Discussion

The list section treats the configuration that returns from this closure as the final separator configuration for the item at the input index path.

## See Also

### Configuring separators

var showsSeparators: Bool

A Boolean value that determines whether the list shows separators between cells.

var separatorConfiguration: UIListSeparatorConfiguration

The section’s preferred configuration for list separators.

struct UIListSeparatorConfiguration

A configuration that controls the list separator appearance in a list section.

typealias ItemSeparatorHandler

A closure that provides granular control over list separator appearance.

