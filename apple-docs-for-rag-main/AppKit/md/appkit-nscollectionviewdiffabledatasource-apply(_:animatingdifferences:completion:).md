

- AppKit
- NSCollectionViewDiffableDataSource
-  apply(\_:animatingDifferences:completion:) 

Instance Method

# apply(\_:animatingDifferences:completion:)

Updates the UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

macOS 10.15.1+

``` source
func apply(
    _ snapshot: NSDiffableDataSourceSnapshot,
    animatingDifferences: Bool = true,
    completion: (() -> Void)? = nil
)
```

## Parameters 

`snapshot`  

The snapshot reflecting the new state of the data in the collection view.

`animatingDifferences`  

If true, the diffable data source computes the difference between the collection view’s current state and the new state in the snapshot, which is an O(*n*) operation, where *n* is the number of items in the snapshot. The differences in the UI between the current state and new state are animated. If false, the collection view UI is set to the new state without any animations, with no additional overhead for computing a diff. Any ongoing item animations are interrupted and the collection view’s content is reloaded immediately.

`completion`  

A closure to be executed when the animations are complete. This closure has no return value and takes no parameters. The system calls this closure from the main queue.

## Discussion

It’s safe to call this method from a background queue, but you must do so consistently in your app. Always call this method exclusively from the main queue or from a background queue.

## See Also

### Updating Data

func snapshot() -> NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

Returns a representation of the current state of the data in the collection view.

