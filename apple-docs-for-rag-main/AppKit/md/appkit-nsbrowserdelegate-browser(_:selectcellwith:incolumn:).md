

- AppKit
- NSBrowserDelegate
-  browser(\_:selectCellWith:inColumn:) 

Instance Method

# browser(\_:selectCellWith:inColumn:)

Asks the delegate to select the cell with the given title in the specified column.

macOS

``` source
@MainActor
optional func browser(
    _ sender: NSBrowser,
    selectCellWith title: String,
    inColumn column: Int
) -> Bool
```

## Parameters 

`sender`  

The browser.

`title`  

The title of the cell to select.

`column`  

The index of the column containing the cell to select.

## Return Value

true if the cell was successfully selected; otherwise, false.

## Discussion

Invoked in response to the setPath(_:) method of NSBrowser being received by `sender`.

## See Also

### Related Documentation

func selectedCell(inColumn: Int) -> Any?

Returns the last (lowest) cell selected in the given column.

### Managing Selection

func browser(NSBrowser, selectRow: Int, inColumn: Int) -> Bool

Asks the delegate to select the cell at the specified row and column location.

func browser(NSBrowser, selectionIndexesForProposedSelection: IndexSet, inColumn: Int) -> IndexSet

Asks the delegate for a set of indexes to select when the user changes the selection in the browser with the keyboard or mouse.

