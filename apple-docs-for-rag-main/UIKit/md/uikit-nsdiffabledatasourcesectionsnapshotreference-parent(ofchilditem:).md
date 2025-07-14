

- UIKit
- NSDiffableDataSourceSectionSnapshotReference
-  parent(ofChildItem:) 

Instance Method

# parent(ofChildItem:)

Finds the parent item of the specified item in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
func parent(ofChildItem childItem: Any) -> Any?
```

## See Also

### Getting item metrics

func index(ofItem: Any) -> Int

Finds the index of the specified item in the section snapshot.

func level(ofItem: Any) -> Int

Finds the hierarchical level of the specified item in the section snapshot.

func containsItem(Any) -> Bool

Indicates whether the section snapshot contains the specified item.

func isVisible(Any) -> Bool

Indicates whether the specified item is currently visible onscreen.

