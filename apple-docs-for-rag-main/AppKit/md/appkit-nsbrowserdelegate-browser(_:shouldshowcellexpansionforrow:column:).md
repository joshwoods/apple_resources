

- AppKit
- NSBrowserDelegate
-  browser(\_:shouldShowCellExpansionForRow:column:) 

Instance Method

# browser(\_:shouldShowCellExpansionForRow:column:)

Invoked to allow the delegate to control cell expansion for a specific row and column.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    shouldShowCellExpansionForRow row: Int,
    column: Int
) -> Bool
```

## Parameters 

`browser`  

The browser.

`row`  

The index of the row requesting an expansion tooltip.

`column`  

The index of the column containing the requesting row.

## Return Value

true to allow the cell expansion tooltip; false to disallow it.

## Discussion

Cell expansion can occur when the mouse hovers over the specified cell and the cell contents are unable to be fully displayed within the cell. If this method returns YES, the full cell contents will be shown in a special floating tool tip view, otherwise the content is truncated.

