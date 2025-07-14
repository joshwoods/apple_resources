

- AppKit
- NSCollectionView
-  insertSections(\_:) 

Instance Method

# insertSections(\_:)

Inserts new sections at the specified indexes.

macOS 10.11+

``` source
@MainActor
func insertSections(_ sections: IndexSet)
```

## Parameters 

`sections`  

An index set containing the indexes at which you want to insert new sections. This parameter must not be `nil`.

## Discussion

This method tells the collection view to insert the specified sections and update itself. Always update your data source object before calling this method. Calling this method kicks off an update (and possible animations) to add the new sections. Specifically, the collection view asks the layout object for any updated layout attributes related to the new sections or any existing sections. If the layout attributes of any visible items changed, those changes are animated into place.

When inserting or deleting multiple sections and items, you can animate all of your changes at once using the performBatchUpdates(_:completionHandler:) method.

## See Also

### Inserting, Moving, Deleting, and Collapsing Sections

func moveSection(Int, toSection: Int)

Moves a section from its current location to a new location.

func deleteSections(IndexSet)

Deletes the specified sections and their contained items.

func toggleSectionCollapse(Any)

Collapses the section in which the sender resides into a single horizontally scrollable row.

