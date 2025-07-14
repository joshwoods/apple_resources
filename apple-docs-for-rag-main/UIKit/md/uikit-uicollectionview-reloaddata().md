

- UIKit
- UICollectionView
-  reloadData() 

Instance Method

# reloadData()

Reloads all of the data for the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func reloadData()
```

## Discussion

Call this method sparingly when you need to reload all of the items in the collection view. This causes the collection view to discard any currently visible items (including placeholders) and recreate items based on the current state of the data source object. For efficiency, the collection view only displays those cells and supplementary views that are visible. If the collection data shrinks as a result of the reload, the collection view adjusts its scrolling offsets accordingly.

You shouldn’t call this method in the middle of animation blocks where items are being inserted or deleted. Insertions and deletions automatically cause the collection’s data to be updated appropriately.

## See Also

### Reloading content

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the collection view contains drop placeholders or is reordering its items as part of handling a drop.

func reconfigureItems(at: [IndexPath])

Updates the data for the items at the index paths you specify, preserving the existing cells for the items.

func reloadSections(IndexSet)

Reloads the data in the specified sections of the collection view.

func reloadItems(at: [IndexPath])

Reloads just the items at the specified index paths.

