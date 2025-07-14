

- UIKit
- UITableView
-  deleteSections(\_:with:) 

Instance Method

# deleteSections(\_:with:)

Deletes one or more sections in the table view, with an option to animate the deletion.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func deleteSections(
    _ sections: IndexSet,
    with animation: UITableView.RowAnimation
)
```

## Parameters 

`sections`  

An index set that specifies the sections to delete from the table view. If a section exists after the specified index location, it is moved up one index location.

`animation`  

A constant that either specifies the kind of animation to perform when deleting the section or requests no animation. See UITableView.RowAnimation for descriptions of the constants.

## Discussion

When this method when is called in an animation block defined by the beginUpdates() and endUpdates() methods, `UITableView` defers any insertions of rows or sections until after it has handled the deletions of rows or sections. This order is followed regardless how the insertion and deletion method calls are ordered. This is unlike inserting or removing an item in a mutable array, in which the operation can affect the array index used for the successive insertion or removal operation. For more on this subject, see Batch Insertion, Deletion, and Reloading of Rows and Sections in Table View Programming Guide for iOS.

## See Also

### Related Documentation

func reloadSections(IndexSet, with: UITableView.RowAnimation)

Reloads the specified sections using the provided animation effect.

### Inserting, deleting, and moving rows and sections

func insertRows(at: [IndexPath], with: UITableView.RowAnimation)

Inserts rows in the table view at the locations that an array of index paths identifies, with an option to animate the insertion.

func deleteRows(at: [IndexPath], with: UITableView.RowAnimation)

Deletes the rows that an array of index paths identifies, with an option to animate the deletion.

func insertSections(IndexSet, with: UITableView.RowAnimation)

Inserts one or more sections in the table view, with an option to animate the insertion.

enum RowAnimation

The type of animation to use when inserting or deleting rows.

func moveRow(at: IndexPath, to: IndexPath)

Moves the row at a specified location to a destination location.

func moveSection(Int, toSection: Int)

Moves a section to a new location in the table view.

