

- AppKit
- NSBrowserDelegate
-  browser(\_:typeSelectStringForRow:inColumn:) 

Instance Method

# browser(\_:typeSelectStringForRow:inColumn:)

Sent to the delegate to get the keyboard-based selection (type select) string for the specified row and column.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    typeSelectStringForRow row: Int,
    inColumn column: Int
) -> String?
```

## Parameters 

`browser`  

The browser.

`row`  

The row index.

`column`  

The column index.

## Return Value

The keyboard-based selection string.

## Discussion

Returning the empty string or `nil` (for example, when the cell does not contain text) specifies that the ``` [``column ```, ``` row``] ``` cell has no text to search.

If the delegate does not implement this method, all cells with text are searched, and the browser determines the keyboard-based selection text by sending stringValue to the cell specified by `column` and `row`.

## See Also

### Managing Selection Behavior

func browser(NSBrowser, shouldTypeSelectFor: NSEvent, withCurrentSearch: String?) -> Bool

Sent to the delegate to determine whether keyboard-based selection (type select) for a given event and search string should proceed.

func browser(NSBrowser, nextTypeSelectMatchFromRow: Int, toRow: Int, inColumn: Int, for: String?) -> Int

Sent to the delegate to customize a browser’s keyboard-based selection (type select) behavior.

