

- UIKit
- UICollectionLayoutListConfiguration
-  UICollectionLayoutListConfiguration.ItemSeparatorHandler 

Type Alias

# UICollectionLayoutListConfiguration.ItemSeparatorHandler

A closure that provides granular control over list separator appearance.

iOS 14.5+iPadOS 14.5+Mac CatalystvisionOS

``` source
typealias ItemSeparatorHandler = (IndexPath, UIListSeparatorConfiguration) -> UIListSeparatorConfiguration
```

## Parameters 

`indexPath`  

The IndexPath of the cell to configure separators for.

`sectionSeparatorConfiguration`  

The list section’s separator configuration for the cell at `indexPath`. This configuration contains the values for separator visibility and insets according to the current state of the item.

## Return Value

The configuration to use for the separators at `indexPath`.

## See Also

### Configuring separators

var showsSeparators: Bool

A Boolean value that determines whether the list shows separators between cells.

var separatorConfiguration: UIListSeparatorConfiguration

The section’s preferred configuration for list separators.

struct UIListSeparatorConfiguration

A configuration that controls the list separator appearance in a list section.

var itemSeparatorHandler: UICollectionLayoutListConfiguration.ItemSeparatorHandler?

The closure that provides granular control over the list separator appearance of each item.

