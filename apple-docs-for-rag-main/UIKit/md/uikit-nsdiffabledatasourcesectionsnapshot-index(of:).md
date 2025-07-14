

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  index(of:) 

Instance Method

# index(of:)

Finds the index of the specified item in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
func index(of item: ItemIdentifierType) -> Int?
```

## See Also

### Getting item metrics

func level(of: ItemIdentifierType) -> Int

Finds the hierarchical level of the specified item in the section snapshot.

func parent(of: ItemIdentifierType) -> ItemIdentifierType?

Finds the parent item of the specified item in the section snapshot.

func contains(ItemIdentifierType) -> Bool

Indicates whether the section snapshot contains the specified item.

func isVisible(ItemIdentifierType) -> Bool

Indicates whether the specified item is currently visible onscreen.

