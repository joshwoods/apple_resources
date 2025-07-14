

- AppKit
- NSBrowserDelegate
-  browser(\_:didChangeLastColumn:toColumn:) 

Instance Method

# browser(\_:didChangeLastColumn:toColumn:)

Tells the delegate that the browser’s last column changed.

macOS

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    didChangeLastColumn oldLastColumn: Int,
    toColumn column: Int
)
```

## Parameters 

`browser`  

The browser.

`oldLastColumn`  

The index of the old last column.

`column`  

The index of the new last column.

## See Also

### Managing Columns

func browser(NSBrowser, createRowsForColumn: Int, in: NSMatrix)

Creates a row in the given matrix for each row of data in the specified column of the browser.

func browser(NSBrowser, willDisplayCell: Any, atRow: Int, column: Int)

Gives the delegate the opportunity to modify the specified cell at the given row and column location before the browser displays it.

