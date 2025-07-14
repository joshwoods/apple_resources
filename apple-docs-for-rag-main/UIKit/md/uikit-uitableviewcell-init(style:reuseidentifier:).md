

- UIKit
- UITableViewCell
-  init(style:reuseIdentifier:) 

Initializer

# init(style:reuseIdentifier:)

Initializes a table cell with a style and a reuse identifier and returns it to the caller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    style: UITableViewCell.CellStyle,
    reuseIdentifier: String?
)
```

## Parameters 

`style`  

A constant indicating a cell style. See UITableViewCell.CellStyle for descriptions of these constants.

`reuseIdentifier`  

A string used to identify the cell object if it is to be reused for drawing multiple rows of a table view. Pass `nil` if the cell object is not to be reused. You should use the same reuse identifier for all cells of the same form.

## Return Value

An initialized UITableViewCell object or `nil` if the object could not be created.

## Discussion

This method is the designated initializer for the class. The reuse identifier is associated with those cells (rows) of a table view that have the same general configuration, minus cell content. In its implementation of tableView(_:cellForRowAt:), the table view’s data source calls the `UITableView` method dequeueReusableCell(withIdentifier:), passing in a reuse identifier, to obtain the cell object to use as the basis for the current row.

If you want a table cell that has a configuration different that those defined by `UITableViewCell` for `style`, you must create your own custom cell. If you want to set the row height of cells on an individual basis, implement the delegate method tableView(_:heightForRowAt:).

## See Also

### Creating a table view cell

enum CellStyle

An enumeration for the various styles of cells.

init?(coder: NSCoder)

Creates a table view from data in an unarchiver.

