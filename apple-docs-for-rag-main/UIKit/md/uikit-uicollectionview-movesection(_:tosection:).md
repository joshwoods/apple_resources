

- UIKit
- UICollectionView
-  moveSection(\_:toSection:) 

Instance Method

# moveSection(\_:toSection:)

Moves a section from one location to another in the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func moveSection(
    _ section: Int,
    toSection newSection: Int
)
```

## Parameters 

`section`  

The index of the section you want to move.

`newSection`  

The index in the collection view that is the destination of the move for the section. The existing section at that location moves up or down to an adjoining index position to make room for it.

## Discussion

Use this method to reorganize existing sections and their contained items. You might do this when you rearrange sections within your data source object or in response to user interactions with the collection view. The collection view updates the layout as needed to account for the move, animating new views into position as needed.

You can also call this method from a block passed to the performBatchUpdates(_:completion:) method when you want to animate multiple separate changes into place at the same time. See the description of that method for more information.

## See Also

### Inserting, moving, and deleting sections

func insertSections(IndexSet)

Inserts new sections at the specified indexes.

func deleteSections(IndexSet)

Deletes the sections at the specified indexes.

