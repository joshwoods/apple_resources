

- UIKit
- UICollectionView
-  reloadSections(\_:) 

Instance Method

# reloadSections(\_:)

Reloads the data in the specified sections of the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func reloadSections(_ sections: IndexSet)
```

## Parameters 

`sections`  

The indexes of the sections to reload.

## Discussion

Call this method to selectively reload only the items in the specified sections. This causes the collection view to discard any cells associated with those items and redisplay them. This method also discards any placeholders in the specified sections.

## See Also

### Reloading content

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the collection view contains drop placeholders or is reordering its items as part of handling a drop.

func reconfigureItems(at: [IndexPath])

Updates the data for the items at the index paths you specify, preserving the existing cells for the items.

func reloadData()

Reloads all of the data for the collection view.

func reloadItems(at: [IndexPath])

Reloads just the items at the specified index paths.

