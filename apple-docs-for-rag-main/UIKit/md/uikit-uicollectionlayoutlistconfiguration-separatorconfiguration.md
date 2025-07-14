

- UIKit
- UICollectionLayoutListConfiguration
-  separatorConfiguration 

Instance Property

# separatorConfiguration

The section’s preferred configuration for list separators.

iOS 14.5+iPadOS 14.5+Mac CatalystvisionOS

``` source
var separatorConfiguration: UIListSeparatorConfiguration { get set }
```

## Discussion

This configuration only takes effect if showsSeparators is true.

For more granular control over list separator appearance, use itemSeparatorHandler.

## See Also

### Configuring separators

var showsSeparators: Bool

A Boolean value that determines whether the list shows separators between cells.

struct UIListSeparatorConfiguration

A configuration that controls the list separator appearance in a list section.

var itemSeparatorHandler: UICollectionLayoutListConfiguration.ItemSeparatorHandler?

The closure that provides granular control over the list separator appearance of each item.

typealias ItemSeparatorHandler

A closure that provides granular control over list separator appearance.

