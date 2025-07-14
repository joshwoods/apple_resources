

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  level(of:) 

Instance Method

# level(of:)

Finds the hierarchical level of the specified item in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
func level(of item: ItemIdentifierType) -> Int
```

## Discussion

A level of `0` means the item is at the root level of the section snapshot.

## See Also

### Getting item metrics

func index(of: ItemIdentifierType) -> Int?

Finds the index of the specified item in the section snapshot.

func parent(of: ItemIdentifierType) -> ItemIdentifierType?

Finds the parent item of the specified item in the section snapshot.

func contains(ItemIdentifierType) -> Bool

Indicates whether the section snapshot contains the specified item.

func isVisible(ItemIdentifierType) -> Bool

Indicates whether the specified item is currently visible onscreen.

