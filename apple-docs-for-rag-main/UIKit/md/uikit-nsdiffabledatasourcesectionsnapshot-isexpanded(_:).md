

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  isExpanded(\_:) 

Instance Method

# isExpanded(\_:)

Indicates whether the item with the specified identifier is in an expanded state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
func isExpanded(_ item: ItemIdentifierType) -> Bool
```

## Discussion

This expansion state persists along with the section snapshot.

## See Also

### Expanding and collapsing items

func expand([ItemIdentifierType])

Expands the specified items in the section snapshot.

func collapse([ItemIdentifierType])

Collapses the specified items in the section snapshot.

