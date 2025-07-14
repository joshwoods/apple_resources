

- UIKit
- UITableView
-  deleteRows(at:with:) 

Instance Method

# deleteRows(at:with:)

Deletes the rows that an array of index paths identifies, with an option to animate the deletion.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func deleteRows(
    at indexPaths: [IndexPath],
    with animation: UITableView.RowAnimation
)
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects identifying the rows to delete.

`animation`  

A constant that indicates how the deletion is to be animated, for example, fade out or slide out from the bottom. See UITableView.RowAnimation for descriptions of these constants.

## Discussion

When this method is called in an animation block defined by the beginUpdates() and endUpdates() methods, `UITableView` defers any insertions of rows or sections until after it has handled the deletions of rows or sections. This order is followed regardless how the insertion and deletion method calls are ordered. This is unlike inserting or removing an item in a mutable array, in which the operation can affect the array index used for the successive insertion or removal operation. For more on this subject, see Batch Insertion, Deletion, and Reloading of Rows and Sections in Table View Programming Guide for iOS.

## See Also

### Related Documentation

func reloadRows(at: [IndexPath], with: UITableView.RowAnimation)

Reloads the specified rows using the provided animation effect.

### Inserting, deleting, and moving rows and sections

func insertRows(at: [IndexPath], with: UITableView.RowAnimation)

Inserts rows in the table view at the locations that an array of index paths identifies, with an option to animate the insertion.

func insertSections(IndexSet, with: UITableView.RowAnimation)

Inserts one or more sections in the table view, with an option to animate the insertion.

func deleteSections(IndexSet, with: UITableView.RowAnimation)

Deletes one or more sections in the table view, with an option to animate the deletion.

enum RowAnimation

The type of animation to use when inserting or deleting rows.

func moveRow(at: IndexPath, to: IndexPath)

Moves the row at a specified location to a destination location.

func moveSection(Int, toSection: Int)

Moves a section to a new location in the table view.

