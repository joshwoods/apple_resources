

- UIKit
- UICollectionView
-  hasUncommittedUpdates 

Instance Property

# hasUncommittedUpdates

A Boolean value that indicates whether the collection view contains drop placeholders or is reordering its items as part of handling a drop.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var hasUncommittedUpdates: Bool { get }
```

## Discussion

When the value of this property is true, avoid making any significant changes to the collection view. Specifically, don’t reload the collection view’s data, as doing so deletes all placeholders and recreates items from the data source.

## See Also

### Reloading content

func reconfigureItems(at: [IndexPath])

Updates the data for the items at the index paths you specify, preserving the existing cells for the items.

func reloadData()

Reloads all of the data for the collection view.

func reloadSections(IndexSet)

Reloads the data in the specified sections of the collection view.

func reloadItems(at: [IndexPath])

Reloads just the items at the specified index paths.

