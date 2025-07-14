

- UIKit
- UICollectionLayoutListConfiguration
-  UICollectionLayoutListConfiguration.SwipeActionsConfigurationProvider 

Type Alias

# UICollectionLayoutListConfiguration.SwipeActionsConfigurationProvider

A closure that configures the swipe actions for a cell.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
typealias SwipeActionsConfigurationProvider = (IndexPath) -> UISwipeActionsConfiguration?
```

## See Also

### Customizing swipe actions

var leadingSwipeActionsConfigurationProvider: UICollectionLayoutListConfiguration.SwipeActionsConfigurationProvider?

The closure that provides the set of actions to display when swiping on the leading edge of the cell.

var trailingSwipeActionsConfigurationProvider: UICollectionLayoutListConfiguration.SwipeActionsConfigurationProvider?

The closure that provides the set of actions to display when swiping on the trailing edge of the cell.

