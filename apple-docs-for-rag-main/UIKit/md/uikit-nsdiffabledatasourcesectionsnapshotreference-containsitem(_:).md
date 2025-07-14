

- UIKit
- NSDiffableDataSourceSectionSnapshotReference
-  containsItem(\_:) 

Instance Method

# containsItem(\_:)

Indicates whether the section snapshot contains the specified item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
func containsItem(_ item: Any) -> Bool
```

## See Also

### Getting item metrics

func index(ofItem: Any) -> Int

Finds the index of the specified item in the section snapshot.

func level(ofItem: Any) -> Int

Finds the hierarchical level of the specified item in the section snapshot.

func parent(ofChildItem: Any) -> Any?

Finds the parent item of the specified item in the section snapshot.

func isVisible(Any) -> Bool

Indicates whether the specified item is currently visible onscreen.

