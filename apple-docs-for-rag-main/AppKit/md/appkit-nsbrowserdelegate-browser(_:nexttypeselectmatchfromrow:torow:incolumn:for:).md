

- AppKit
- NSBrowserDelegate
-  browser(\_:nextTypeSelectMatchFromRow:toRow:inColumn:for:) 

Instance Method

# browser(\_:nextTypeSelectMatchFromRow:toRow:inColumn:for:)

Sent to the delegate to customize a browser’s keyboard-based selection (type select) behavior.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    nextTypeSelectMatchFromRow startRow: Int,
    toRow endRow: Int,
    inColumn column: Int,
    for searchString: String?
) -> Int
```

## Parameters 

`browser`  

The browser.

`startRow`  

The beginning of the row set to search.

`endRow`  

The end of the row set to search. This value can be less than `startRowIndex` when the search wraps around to the beginning.

`column`  

The column containing the rows being searched.

`searchString`  

The keyboard-based selection string. It is `nil` when no keyboard-based selection has begun.

## Return Value

The index of the first row that matches `searchString` between `startRowIndex` and `endRowIndex` - 1, or `-1` if there is no match.

## See Also

### Managing Selection Behavior

func browser(NSBrowser, shouldTypeSelectFor: NSEvent, withCurrentSearch: String?) -> Bool

Sent to the delegate to determine whether keyboard-based selection (type select) for a given event and search string should proceed.

func browser(NSBrowser, typeSelectStringForRow: Int, inColumn: Int) -> String?

Sent to the delegate to get the keyboard-based selection (type select) string for the specified row and column.

