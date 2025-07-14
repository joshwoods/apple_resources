

- UIKit
- UITableView
-  dequeueReusableCell(withIdentifier:) 

Instance Method

# dequeueReusableCell(withIdentifier:)

Returns a reusable table-view cell object after locating it by its identifier.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dequeueReusableCell(withIdentifier identifier: String) -> UITableViewCell?
```

## Parameters 

`identifier`  

A string identifying the cell object to be reused. This parameter must not be `nil`.

## Return Value

A UITableViewCell object with the associated `identifier`, or `nil` if no such object exists in the reusable-cell queue.

## Discussion

For performance reasons, a table view’s data source should generally reuse UITableViewCell objects when it assigns cells to rows in its tableView(_:cellForRowAt:) method. A table view maintains a queue or list of UITableViewCell objects that the data source has marked for reuse. Call this method from your data source object when asked to provide a new cell for the table view. This method dequeues an existing cell if one is available or creates a new one using the class or nib file you previously registered. If no cell is available for reuse and you didn’t register a class or nib file, this method returns `nil`.

If you registered a class for the specified `identifier` and a new cell must be created, this method initializes the cell by calling its init(style:reuseIdentifier:) method. For nib-based cells, this method loads the cell object from the provided nib file. If an existing cell was available for reuse, this method calls the cell’s prepareForReuse() method instead.

## See Also

### Recycling table view cells

func register(UINib?, forCellReuseIdentifier: String)

Registers a nib object that contains a cell with the table view under a specified identifier.

func register(AnyClass?, forCellReuseIdentifier: String)

Registers a class to use in creating new table cells.

func dequeueReusableCell(withIdentifier: String, for: IndexPath) -> UITableViewCell

Returns a reusable table-view cell object for the specified reuse identifier and adds it to the table.

