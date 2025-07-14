

- UIKit
- UITableView
-  dequeueReusableCell(withIdentifier:for:) 

Instance Method

# dequeueReusableCell(withIdentifier:for:)

Returns a reusable table-view cell object for the specified reuse identifier and adds it to the table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dequeueReusableCell(
    withIdentifier identifier: String,
    for indexPath: IndexPath
) -> UITableViewCell
```

## Parameters 

`identifier`  

A string identifying the cell object to be reused. This parameter must not be `nil`.

`indexPath`  

The index path specifying the location of the cell. Always specify the index path provided to you by your data source object. This method uses the index path to perform additional configuration based on the cell’s position in the table view.

## Return Value

A UITableViewCell object with the associated reuse identifier. This method always returns a valid cell.

## Mentioned in 

Configuring the cells for your table

Filling a table with data

## Discussion

Call this method only from the tableView(_:cellForRowAt:) method of your table view data source object. This method returns an existing cell of the specified type, if one is available, or it creates and returns a new cell using the class or storyboard you provided earlier. Don’t call this method outside of your data source’s tableView(_:cellForRowAt:) method. If you need to create cells at other times, call dequeueReusableCell(withIdentifier:) instead.

Important

You must specify a cell with a matching identifier in your storyboard file. You may also register a class or nib file using the register(_:forCellReuseIdentifier:) or register(_:forCellReuseIdentifier:) method, but must do so before calling this method.

When creating new cells from your storyboard or nib file, this method loads the cell object and initializes it using its init(coder:) method. When creating cells from a registered class, this method creates the cell and initializes it by calling its init(style:reuseIdentifier:) method. For nib-based cells, this method loads the cell object from the provided nib file. If an existing cell was available for reuse, this method calls the cell’s prepareForReuse() method instead.

## See Also

### Recycling table view cells

func register(UINib?, forCellReuseIdentifier: String)

Registers a nib object that contains a cell with the table view under a specified identifier.

func register(AnyClass?, forCellReuseIdentifier: String)

Registers a class to use in creating new table cells.

func dequeueReusableCell(withIdentifier: String) -> UITableViewCell?

Returns a reusable table-view cell object after locating it by its identifier.

