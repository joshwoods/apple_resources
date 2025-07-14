

- UIKit
- UICollectionView
-  insertSections(\_:) 

Instance Method

# insertSections(\_:)

Inserts new sections at the specified indexes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func insertSections(_ sections: IndexSet)
```

## Parameters 

`sections`  

An index set containing the indexes of the sections you want to insert. This parameter must not be `nil`.

## Discussion

Use this method to insert one or more sections into the collection view. This method adds the sections, and it is up to your data source to report the number of items in each section when asked for the information. The collection view then uses that information to get updated layout attributes for the newly inserted sections and items. If the insertions cause a change in the collection view’s visible content, those changes are animated into place.

You can also call this method from a block passed to the performBatchUpdates(_:completion:) method when you want to animate multiple separate changes into place at the same time. See the description of that method for more information.

## See Also

### Inserting, moving, and deleting sections

func moveSection(Int, toSection: Int)

Moves a section from one location to another in the collection view.

func deleteSections(IndexSet)

Deletes the sections at the specified indexes.

