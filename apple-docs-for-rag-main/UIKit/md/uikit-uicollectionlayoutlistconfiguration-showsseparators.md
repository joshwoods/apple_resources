

- UIKit
- UICollectionLayoutListConfiguration
-  showsSeparators 

Instance Property

# showsSeparators

A Boolean value that determines whether the list shows separators between cells.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
var showsSeparators: Bool { get set }
```

## See Also

### Configuring separators

var separatorConfiguration: UIListSeparatorConfiguration

The section’s preferred configuration for list separators.

struct UIListSeparatorConfiguration

A configuration that controls the list separator appearance in a list section.

var itemSeparatorHandler: UICollectionLayoutListConfiguration.ItemSeparatorHandler?

The closure that provides granular control over the list separator appearance of each item.

typealias ItemSeparatorHandler

A closure that provides granular control over list separator appearance.

