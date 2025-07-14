

- AppKit
- NSBrowserDelegate
-  browser(\_:selectionIndexesForProposedSelection:inColumn:) 

Instance Method

# browser(\_:selectionIndexesForProposedSelection:inColumn:)

Asks the delegate for a set of indexes to select when the user changes the selection in the browser with the keyboard or mouse.

macOS 10.6+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    selectionIndexesForProposedSelection proposedSelectionIndexes: IndexSet,
    inColumn column: Int
) -> IndexSet
```

## Parameters 

`browser`  

The browser.

`proposedSelectionIndexes`  

The set of indexes of the items in the proposed selection.

`column`  

The column index of the column containing the selection.

## Return Value

The set of indexes of the items that should be selected.

## Discussion

This method may be called multiple times, with one new index added to the previous selection, to see whether a particular index can be selected when the user is extending the selection with the keyboard or mouse. The `proposedSelectionIndexes` parameter contains the entire selection, and you can return the existing selection if you do not want to change it. This method works only for item-based browsers.

## See Also

### Managing Selection

func browser(NSBrowser, selectCellWith: String, inColumn: Int) -> Bool

Asks the delegate to select the cell with the given title in the specified column.

func browser(NSBrowser, selectRow: Int, inColumn: Int) -> Bool

Asks the delegate to select the cell at the specified row and column location.

