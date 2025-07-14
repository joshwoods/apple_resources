

- AppKit
- NSCollectionView
-  toggleSectionCollapse(\_:) 

Instance Method

# toggleSectionCollapse(\_:)

Collapses the section in which the sender resides into a single horizontally scrollable row.

macOS 10.12+

``` source
@IBAction @MainActor
func toggleSectionCollapse(_ sender: Any)
```

## Parameters 

`sender`  

The object that requested the action.

## Discussion

The icon view in Finder offers this type of collapsible section behavior when users choose the Show Less and Show More buttons. To enable this behavior, your header view must conform to the `NSCollectionViewSectionHeaderView` protocol, because the collection view uses the `sectionCollapseButton` property to identify the button that controls the collapse action.

## See Also

### Inserting, Moving, Deleting, and Collapsing Sections

func insertSections(IndexSet)

Inserts new sections at the specified indexes.

func moveSection(Int, toSection: Int)

Moves a section from its current location to a new location.

func deleteSections(IndexSet)

Deletes the specified sections and their contained items.

