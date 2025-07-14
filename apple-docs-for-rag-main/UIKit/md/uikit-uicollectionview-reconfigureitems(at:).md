

- UIKit
- UICollectionView
-  reconfigureItems(at:) 

Instance Method

# reconfigureItems(at:)

Updates the data for the items at the index paths you specify, preserving the existing cells for the items.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func reconfigureItems(at indexPaths: [IndexPath])
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects identifying the items you want to update.

## Discussion

To update the contents of existing (including prefetched) cells without replacing them with new cells, use this method instead of reloadItems(at:). For optimal performance, choose to reconfigure items instead of reloading items unless you have an explicit need to replace the existing cell with a new cell.

Your cell provider must dequeue the same type of cell for the provided index path, and must return the same existing cell for a given index path. Because this method reconfigures existing cells, the collection view doesn’t call prepareForReuse() for each cell dequeued. If you need to return a different type of cell for an index path, use reloadItems(at:) instead.

If your cells are self-sizing, the collection view resizes your cells after reconfiguring them.

By default, the collection view animates any size or layout changes that result from reconfiguration. To reconfigure cells without animation, use `UIView`’s performWithoutAnimation(_:) when you call this method. Alternatively, to avoid animations when setting specific properties, use performWithoutAnimation(_:) in your cell configuration logic.

If your collection view uses a custom implementation of `UICollectionViewDataSource`, use this method. If your collection view uses a diffable data source, use reconfigureItems(_:) (Swift) or reconfigureItems(withIdentifiers:) (Objective-C) on `NSDiffableDataSourceSnapshot` instead.

## See Also

### Reloading content

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the collection view contains drop placeholders or is reordering its items as part of handling a drop.

func reloadData()

Reloads all of the data for the collection view.

func reloadSections(IndexSet)

Reloads the data in the specified sections of the collection view.

func reloadItems(at: [IndexPath])

Reloads just the items at the specified index paths.

