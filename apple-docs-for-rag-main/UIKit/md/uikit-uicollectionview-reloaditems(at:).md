

- UIKit
- UICollectionView
-  reloadItems(at:) 

Instance Method

# reloadItems(at:)

Reloads just the items at the specified index paths.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func reloadItems(at indexPaths: [IndexPath])
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects identifying the items you want to update.

## Discussion

Call this method to selectively reload only the specified items. This causes the collection view to discard any cells associated with those items and redisplay them.

## See Also

### Reloading content

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the collection view contains drop placeholders or is reordering its items as part of handling a drop.

func reconfigureItems(at: [IndexPath])

Updates the data for the items at the index paths you specify, preserving the existing cells for the items.

func reloadData()

Reloads all of the data for the collection view.

func reloadSections(IndexSet)

Reloads the data in the specified sections of the collection view.

