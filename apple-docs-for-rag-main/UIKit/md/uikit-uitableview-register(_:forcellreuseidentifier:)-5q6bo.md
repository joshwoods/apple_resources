

- UIKit
- UITableView
-  register(\_:forCellReuseIdentifier:) 

Instance Method

# register(\_:forCellReuseIdentifier:)

Registers a nib object that contains a cell with the table view under a specified identifier.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func register(
    _ nib: UINib?,
    forCellReuseIdentifier identifier: String
)
```

## Parameters 

`nib`  

A nib object that specifies the nib file to use to create the cell.

`identifier`  

The reuse identifier for the cell. This parameter must not be `nil` and must not be an empty string.

## Discussion

Before dequeueing any cells, call this method or the register(_:forCellReuseIdentifier:) method to tell the table view how to create new cells. If a cell of the specified type isn’t currently in a reuse queue, the table view uses the provided information to create a new cell object automatically.

If you previously registered a class or nib file with the same reuse identifier, the nib you specify in the `nib` parameter replaces the old entry. You may specify `nil` for `nib` if you want to unregister the nib from the specified reuse identifier.

## See Also

### Related Documentation

func tableView(UITableView, cellForRowAt: IndexPath) -> UITableViewCell

Asks the data source for a cell to insert in a particular location of the table view.

**Required**

### Recycling table view cells

func register(AnyClass?, forCellReuseIdentifier: String)

Registers a class to use in creating new table cells.

func dequeueReusableCell(withIdentifier: String, for: IndexPath) -> UITableViewCell

Returns a reusable table-view cell object for the specified reuse identifier and adds it to the table.

func dequeueReusableCell(withIdentifier: String) -> UITableViewCell?

Returns a reusable table-view cell object after locating it by its identifier.

