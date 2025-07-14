

- AppKit
- NSBrowserDelegate
-  browser(\_:selectRow:inColumn:) 

Instance Method

# browser(\_:selectRow:inColumn:)

Asks the delegate to select the cell at the specified row and column location.

macOS

``` source
@MainActor
optional func browser(
    _ sender: NSBrowser,
    selectRow row: Int,
    inColumn column: Int
) -> Bool
```

## Parameters 

`sender`  

The browser.

`row`  

The index of the row containing the cell to select.

`column`  

The index of the column containing the cell to select.

## Return Value

true if the cell was selected; otherwise, false.

## Discussion

Invoked in response to selectRow(_:inColumn:) of NSBrowser being received by `sender`.

## See Also

### Related Documentation

func selectRow(Int, inColumn: Int)

Selects the cell at the specified row and column index.

func selectedRow(inColumn: Int) -> Int

Returns the row index of the selected cell in the specified column.

### Managing Selection

func browser(NSBrowser, selectCellWith: String, inColumn: Int) -> Bool

Asks the delegate to select the cell with the given title in the specified column.

func browser(NSBrowser, selectionIndexesForProposedSelection: IndexSet, inColumn: Int) -> IndexSet

Asks the delegate for a set of indexes to select when the user changes the selection in the browser with the keyboard or mouse.

