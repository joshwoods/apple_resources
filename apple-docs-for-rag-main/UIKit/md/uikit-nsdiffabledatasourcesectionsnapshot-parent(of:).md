

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  parent(of:) 

Instance Method

# parent(of:)

Finds the parent item of the specified item in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
func parent(of child: ItemIdentifierType) -> ItemIdentifierType?
```

## See Also

### Getting item metrics

func index(of: ItemIdentifierType) -> Int?

Finds the index of the specified item in the section snapshot.

func level(of: ItemIdentifierType) -> Int

Finds the hierarchical level of the specified item in the section snapshot.

func contains(ItemIdentifierType) -> Bool

Indicates whether the section snapshot contains the specified item.

func isVisible(ItemIdentifierType) -> Bool

Indicates whether the specified item is currently visible onscreen.

