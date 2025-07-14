

- UIKit
- NSDiffableDataSourceSectionSnapshotReference
-  isExpanded(\_:) 

Instance Method

# isExpanded(\_:)

Indicates whether the item with the specified identifier is in an expanded state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
func isExpanded(_ item: Any) -> Bool
```

## Discussion

This expansion state persists along with the section snapshot.

## See Also

### Expanding and collapsing items

func expandItems([Any])

Expands the specified items in the section snapshot.

func collapseItems([Any])

Collapses the specified items in the section snapshot.

