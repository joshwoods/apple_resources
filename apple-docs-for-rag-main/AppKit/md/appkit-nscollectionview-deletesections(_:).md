

- AppKit
- NSCollectionView
-  deleteSections(\_:) 

Instance Method

# deleteSections(\_:)

Deletes the specified sections and their contained items.

macOS 10.11+

``` source
@MainActor
func deleteSections(_ sections: IndexSet)
```

## Parameters 

`sections`  

An index set containing the indexes of the sections that you want to delete. This parameter must not be `nil`.

## Discussion

Use this method to delete entire sections and their contained items. Always update your data source object before calling this method. Calling this method kicks off an update (and possible animations) to delete the specified sections. Specifically, the collection view asks the layout object for the final layout attributes for any deleted sections and may also ask for updated layout attributes for any remaining sections. If the layout attributes of any visible items changed, those changes are animated into place.

When inserting or deleting multiple sections and items, you can animate all of your changes at once using the performBatchUpdates(_:completionHandler:) method.

## See Also

### Inserting, Moving, Deleting, and Collapsing Sections

func insertSections(IndexSet)

Inserts new sections at the specified indexes.

func moveSection(Int, toSection: Int)

Moves a section from its current location to a new location.

func toggleSectionCollapse(Any)

Collapses the section in which the sender resides into a single horizontally scrollable row.

