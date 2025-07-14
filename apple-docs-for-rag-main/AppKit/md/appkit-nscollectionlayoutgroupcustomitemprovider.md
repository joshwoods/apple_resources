

- AppKit
-  NSCollectionLayoutGroupCustomItemProvider 

Type Alias

# NSCollectionLayoutGroupCustomItemProvider

A closure that creates and returns each of the custom group’s items.

macOS

``` source
typealias NSCollectionLayoutGroupCustomItemProvider = (any NSCollectionLayoutEnvironment) -> [NSCollectionLayoutGroupCustomItem]
```

## Discussion

You use a custom item provider to supply the item arrangement when creating a group using the custom(layoutSize:itemProvider:) initializer.

## See Also

### Advanced layouts

class NSCollectionLayoutGroupCustomItem

An item used in a group with a custom layout arrangement.

